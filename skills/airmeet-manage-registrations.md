---
name: Manage event registrations
description: Add authorized attendees, block/unblock them, and read the participant list.
api: openapi/airmeet-openapi.yml
operations: [authenticate, addAttendee, blockAttendee, unblockAttendee, getParticipants]
---

# Manage event registrations

## Auth
1. `authenticate` — POST `/auth`; send the token as `X-Airmeet-Access-Token`.

## Steps
2. `addAttendee` — POST `/airmeet/{airmeetId}/attendee` with `email`, `firstName`, `lastName`. Set `sendEmailInvite` (default true) and `registerAttendee` (default false) as needed; for hybrid events set `attendance_type` to `IN-PERSON` or `VIRTUAL`. Map custom fields with `customFieldMapping[]` (get field ids from `getCustomFields`).
3. `blockAttendee` — PUT `/airmeet/{airmeetId}/attendee/block` with `attendeeEmail`.
4. `unblockAttendee` — PUT `/airmeet/{airmeetId}/attendee/unblock` with `attendeeEmail`.
5. `getParticipants` — GET `/airmeet/{airmeetId}/participants` to confirm the roster.

## Rules
- `attendeeEmail` is the identity key for block/unblock; there are no numeric attendee ids in these calls.
- No idempotency key — re-adding the same email is not guaranteed safe; check `getParticipants` first.
- `401` means re-authenticate; `400` means a required field is missing.
