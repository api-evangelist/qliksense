---
name: qliksense-reload-an-app
description: >-
  Refresh the data in a Qlik analytics app, either as a one-off reload or as a
  scheduled task, and watch it to completion. Use when asked to reload a Qlik
  app, refresh a dashboard's data, schedule a nightly refresh, or diagnose a
  failed reload.
api: openapi/qliksense-reloads.json, openapi/qliksense-scheduling-tasks.json, openapi/qliksense-apps.json
operations:
  - listTasks
  - createTask
  - startTask
  - getTaskRuns
  - getTaskRunLog
  - getTaskLastRun
generated: '2026-08-29'
method: generated
source: >-
  Grounded in operationIds verified verbatim in
  openapi/qliksense-scheduling-tasks.json. The Reloads API operations are cited
  by METHOD + PATH because openapi/qliksense-reloads.json declares no
  operationId on any of its four operations.
---

# Reload a Qlik analytics app

## Which API to use

Qlik has two overlapping surfaces here and picked a winner in June 2026:

- **Scheduling Tasks API** (`/api/scheduling/tasks`) — current. Namespaced,
  fully operationId'd, models dependency graphs between tasks.
- **Reload Tasks API** (`/api/v1/reload-tasks`) — **deprecated**, superseded by
  Scheduling Tasks (changelog entry 231, 2026-06-26). Do not build on it.
- **Reloads API** (`/api/v1/reloads`) — still current, but for firing and
  cancelling a single ad-hoc reload, not for scheduling.

Prefer Scheduling Tasks for anything recurring.

## One-off reload

1. `POST /api/v1/reloads` with the app id. (No operationId is published for this
   operation — that is a gap in Qlik's contract, not in this skill.)
2. Poll `GET /api/v1/reloads/{reloadId}` until status is terminal.
3. To abort: `POST /api/v1/reloads/{reloadId}/actions/cancel`. This is the only
   reversal available — once a reload completes, the previous data state is not
   restorable through the API.

## Scheduled reload

1. `listTasks` — `GET /api/scheduling/tasks` to see what already exists for the
   app before creating a duplicate.
2. `createTask` — `POST /api/scheduling/tasks` with the app as the resource and
   the schedule.
3. `startTask` — `POST /api/scheduling/tasks/{id}/actions/start` to run it now.
4. `getTaskRuns` / `getTaskLastRun` to check outcome; `getTaskRunLog`
   (`GET /api/scheduling/tasks/{id}/runs/{runId}/log`) for the failure detail.

## Chaining

Task dependency graphs are first-class: `listParentTasks`, `listChildTasks`,
`listAncestorTasks`, `listDescendantTasks` and `listTaskSubgraph` all read the
graph around a task. Use them before deleting a task — `deleteTask` is
permanent and Qlik documents no restore.

## Rules that apply throughout

- `POST /api/v1/reloads` and `createTask` are tier 2 (100/min). Polling reads
  are tier 1 (1,000/min) — but poll with backoff anyway; there are no
  remaining-quota headers, only `Retry-After` on the 429.
- **No idempotency keys.** A retried `createTask` creates a second task. List
  first.
- Reload lifecycle also arrives as events: subscribe a webhook to the reloads
  domain rather than polling. See `asyncapi/qliksense-reloads-asyncapi.json` and
  `asyncapi/qliksense-webhooks.yml`.
