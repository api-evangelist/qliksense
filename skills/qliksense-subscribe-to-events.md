---
name: qliksense-subscribe-to-events
description: >-
  Subscribe to Qlik Cloud tenant events over a webhook, verify the HMAC
  signature, and replay a failed delivery. Use when asked to get notified of
  Qlik changes, wire Qlik into another system in real time, build event-driven
  automation on Qlik, or debug a webhook that is not firing.
api: openapi/qliksense-webhooks.json
operations:
  - listEventTypes
  - listWebhookEntries
  - createWebhook
  - getWebhookDeliveryList
  - getWebhookDelivery
  - resendDelivery
  - deleteWebhook
generated: '2026-08-29'
method: generated
source: >-
  Grounded in operationIds verified verbatim in openapi/qliksense-webhooks.json,
  the 29 AsyncAPI 3.0.0 event documents in asyncapi/, and
  https://qlik.dev/apis/event/verify-webhook-signatures-hmac/.
---

# Subscribe to Qlik Cloud events

Qlik describes its whole event surface in machine-readable AsyncAPI 3.0.0 — 29
documents, 102 message definitions, all in `asyncapi/`. Read the shape there
before you write a handler; you do not have to guess at payloads.

## Steps

1. **Find the event types you want.**
   `listEventTypes` — `GET /api/v1/webhooks/event-types` enumerates what this
   tenant can actually subscribe to right now. Cross-reference the payload
   schema in `asyncapi/qliksense-<domain>-asyncapi.json`.

2. **Check for an existing subscription.**
   `listWebhookEntries` — `GET /api/v1/webhooks`. There are no idempotency keys,
   so creating blind duplicates deliveries.

3. **Create the webhook.**
   `createWebhook` — `POST /api/v1/webhooks` with your URL, the event types, and
   **a secret**. Set the secret. Without one you cannot verify anything.

4. **Verify every delivery.**
   Qlik signs each request with HMAC-SHA256 over the payload using your secret.
   Compare in constant time and reject on mismatch. An unverified endpoint is
   forgeable by anyone who learns the URL.
   Docs: https://qlik.dev/apis/event/verify-webhook-signatures-hmac/

5. **Handle the CloudEvents envelope.**
   Every payload carries CloudEvents 1.0 context attributes (`id`, `source`,
   `specversion`, `type`, `time`, `datacontenttype`) plus Qlik's `userid` and
   `tenantid` extensions. Dispatch on `type` (e.g. `com.qlik.app.softdeleted`),
   and dedupe on `id` — retried deliveries reuse it.

6. **Debug with the delivery log.**
   `getWebhookDeliveryList` — `GET /api/v1/webhooks/{id}/deliveries` shows what
   Qlik tried to send and what your endpoint answered.
   `getWebhookDelivery` for one record, and `resendDelivery`
   (`POST /api/v1/webhooks/{id}/deliveries/{deliveryId}/actions/resend`) to
   replay it after you fix the handler. Replay is the reason to keep the
   subscription alive while debugging rather than deleting and recreating it.

## Watch out for

- **Legacy event fields are being removed** from webhook payloads (deprecation
  notice 2026-05-11). Pin your handler to the CloudEvents attributes and the
  documented `data` shape, not to legacy top-level fields.
- `deleteWebhook` is permanent and takes the delivery history with it.
- Writes here are tier 2 (100/min); the delivery log reads are tier 1.
