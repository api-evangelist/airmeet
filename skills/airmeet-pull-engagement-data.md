---
name: Pull post-event engagement and attendance data
description: Read attendance, poll, Q&A and recording data for an event, handling async exports.
api: openapi/airmeet-openapi.yml
operations: [authenticate, listAirmeets, getAttendees, getPolls, getQuestions, getSessionRecordings]
---

# Pull post-event engagement and attendance data

## Auth
1. `authenticate` — POST `/auth`; send the token as `X-Airmeet-Access-Token`.

## Steps
2. `listAirmeets` — GET `/airmeets` with `pageNumber`/`pageSize` to find the airmeet id.
3. `getAttendees` — GET `/airmeet/{airmeetId}/attendees`. This is asynchronous: it returns a job/URL reference; poll it until the dataset is ready.
4. `getPolls` — GET `/airmeet/{airmeetId}/polls` for poll responses.
5. `getQuestions` — GET `/airmeet/{airmeetId}/questions` for Q&A.
6. `getSessionRecordings` — GET `/airmeet/{airmeetId}/session-recordings` for recording download links.

## Rules
- Async endpoints (`getAttendees`, `getSessionAttendees`, `getBoothAttendance`, `getUtms`, `getEventReplayAttendees`) do not return data inline — expect a reference to poll.
- A `412` on an async read usually means the export is not ready yet; back off and retry.
- Paginate `listAirmeets` with `pageNumber`/`pageSize` rather than assuming one page.
