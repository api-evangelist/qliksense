---
name: qliksense-onboard-user-to-space
description: >-
  Invite a user into a Qlik Cloud tenant and give them working access to a
  shared space. Use when asked to onboard a person to Qlik, grant access to a
  space, or fix "the user can see the tenant but not the content".
api: openapi/qliksense-users.json, openapi/qliksense-spaces.json
operations:
  - inviteUsers
  - getUsers
  - getSpaces
  - createSpace
  - getTypes
  - createSpaceAssignment
  - getSpaceAssignments
generated: '2026-08-29'
method: generated
source: >-
  Grounded in operationIds verified verbatim in openapi/qliksense-users.json and
  openapi/qliksense-spaces.json (harvested from https://qlik.dev/specs/rest/).
---

# Onboard a user into a Qlik Cloud space

Two things must both be true before a person can do anything useful in Qlik
Cloud: they exist in the **tenant**, and they hold a role in a **space**. Tenant
membership alone gets them a hub with nothing in it — this is the single most
common "Qlik access is broken" report.

## Before you start

- Base URL: `https://{tenant}.{region}.qlikcloud.com`
- Auth: `Authorization: Bearer <token>` (API key, OAuth token, or JWT — see
  `authentication/qliksense-authentication.yml`).
- Scope: creating users and space assignments needs `admin.users` and
  `admin.spaces`; reading only needs `admin.users:read` / `admin.spaces:read`.
  See `scopes/qliksense-scopes.yml`.
- The published OpenAPI declares **no** securityScheme, so a generated client
  will not add the Authorization header for you. Add it yourself.

## Steps

1. **Check whether the user already exists.**
   `getUsers` — `GET /api/v1/users?filter=email eq "person@example.com"`.
   The `filter` grammar is SCIM (RFC 7644 §3.4.2.2), not a Qlik invention.
   Follow `links.next.href` if you page; cursors are opaque.

2. **Invite them if they do not.**
   `inviteUsers` — `POST /api/v1/users/actions/invite`. This sends an invitation
   rather than creating an active user directly; the account materialises when
   they accept. `createUser` (`POST /api/v1/users`) exists but is for
   IdP-provisioned flows.

3. **Find or create the target space.**
   `getSpaces` — `GET /api/v1/spaces?filter=name eq "Finance"`.
   If it does not exist, call `getTypes` (`GET /api/v1/spaces/types`) first to
   see which space types the tenant licence allows, then `createSpace`
   (`POST /api/v1/spaces`) with a valid `type`.

4. **Assign the role in the space.**
   `createSpaceAssignment` — `POST /api/v1/spaces/{spaceId}/assignments` with
   the user id and the role. THIS is the step that actually grants access.

5. **Verify.**
   `getSpaceAssignments` — `GET /api/v1/spaces/{spaceId}/assignments` and
   confirm the assignment is present.

## Rules that apply throughout

- **Rate limits.** Reads are tier 1 (1,000/min); every write above is tier 2
  (100/min), evaluated per user per tenant over a rolling 5-minute window. On
  429 read `Retry-After` and wait — there are no remaining-quota headers to
  watch. See `rate-limits/qliksense-rate-limits.yml`.
- **No idempotency keys.** Qlik supports none. A retried `inviteUsers` or
  `createSpaceAssignment` can duplicate. Re-read with `getUsers` /
  `getSpaceAssignments` before retrying rather than firing blind.
- **Errors** arrive as `{"errors":[{"code","title","detail"}]}`, not RFC 9457
  problem+json. See `errors/qliksense-problem-types.yml`.
- **Reversibility.** `deleteSpaceAssignmentById` and `deleteUserById` are
  permanent — Qlik documents no restore window for either. Only analytics apps
  have a documented recovery window. See the `reversibility` block in
  `conventions/qliksense-conventions.yml`.
