---
name: Create and launch an Airmeet event
description: Create an Airmeet event, add a speaker and a session, then start it via the API.
api: openapi/airmeet-openapi.yml
operations: [authenticate, createAirmeet, addSpeaker, createSession, updateAirmeetStatus]
---

# Create and launch an Airmeet event

Use the Airmeet Public API to stand up an event end to end.

## Auth
1. `authenticate` — POST `/auth` with headers `X-Airmeet-Access-Key` and `X-Airmeet-Secret-Key`. Cache the returned `data.token` (valid 30 days). Send it as `X-Airmeet-Access-Token` on every later call.

## Steps
2. `createAirmeet` — POST `/airmeet` with `hostEmail` and `eventName` (plus `startTime`, `endTime`, `timezone`, `eventType`). Capture the returned airmeet id.
3. `addSpeaker` — POST `/airmeet/{airmeetId}/speaker` with `name` and `email`.
4. `createSession` — POST `/airmeet/{airmeetId}/session` with `sessionTitle`, `sessionStartTime`, and `speakerEmails` referencing the speaker you added.
5. `updateAirmeetStatus` — POST `/airmeet/{airmeetId}/status` with `status: ONGOING` to start, and `FINISHED` to end.

## Rules
- Pick the regional base URL that matches your workspace: `api-gateway.airmeet.com/prod` (default), `api-gateway-prod.eu.airmeet.com/prod`, or `api-gateway-prod.us.airmeet.com/prod`.
- There is no idempotency key — do not blindly retry `createAirmeet`/`createSession` on timeout; re-list first to avoid duplicates.
- Errors return `{ "success": false, "message": ... }`; treat `401` as an expired/invalid token and re-authenticate.
