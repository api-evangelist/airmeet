---
name: Subscribe to Airmeet webhook events
description: Register a webhook endpoint against an Airmeet event trigger.
api: openapi/airmeet-openapi.yml
operations: [registerWebhook]
---

# Subscribe to Airmeet webhook events

## Steps
1. `registerWebhook` — POST `/platform-integration/v1/webhook-register` with headers `x-access-key` and `x-secret-key` (note: this endpoint uses the raw key headers, not the `/auth` access token). Body: `name`, `triggerMetaInfoId` (the event type), and `url` (your HTTPS receiver). Optional: `description`, `platformName`.

## Rules
- Choose the trigger via `triggerMetaInfoId` — e.g. `trigger.airmeet.attendee.added`, `trigger.session.attendee.joined`, `trigger.airmeet.polls`, `trigger.attendee.entered_airmeet` (see asyncapi/airmeet-webhooks-asyncapi.yml for the full 24+ list).
- Event-specific triggers append an `airmeetId` query parameter to your registered URL; some also send `sessionId`.
- Payloads are `application/json`. No signature/verification header is documented, so validate on a secret path or allowlist Airmeet source ranges.
