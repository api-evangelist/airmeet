# Airmeet

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Airmeet is a virtual, hybrid and in-person events platform used to run webinars, conferences, summits, meetups, workshops and trade shows with interactive stages, networking lounges, booths, polls, Q&A and engagement analytics. Its Public API lets developers create and manage events (Airmeets), sessions, speakers, booths and event series; manage registrations (add, block and unblock attendees with custom fields); pull engagement and attendance data including polls, questions, UTMs, recordings and replay attendance; and subscribe to 24+ webhook event triggers. Authentication is a two-step flow: exchange an access key and secret key for a 30-day access token, then send it as the X-Airmeet-Access-Token header. The API is served from regional gateways (default Mumbai, EU and US). Airmeet is backed by Accel, Prosus Ventures and Redpoint Ventures.

**Areas:** Company · Cloud Saas · Event · Virtual Events · Webinars · Event Management · Community · Webhook

## Airmeet on APIs.io

Everything profiled for Airmeet is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/airmeet/](https://apis.io/providers/airmeet/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Airmeet Authentication API](https://apis.io/apis/airmeet/airmeet-authentication-api/) — Exchange access/secret keys for an access token.
- [Airmeet Event Details API](https://apis.io/apis/airmeet/airmeet-event-details-api/) — Read events, participants, sessions, engagement and attendance data.
- [Airmeet Manage Event API](https://apis.io/apis/airmeet/airmeet-manage-event-api/) — Create and manage events, speakers, sessions, booths and landing pages.
- [Airmeet Manage Event Series API](https://apis.io/apis/airmeet/airmeet-manage-event-series-api/) — List event series and the events within a series.
- [Airmeet Manage Registrations API](https://apis.io/apis/airmeet/airmeet-manage-registrations-api/) — Add authorized attendees and block or unblock them.
- [Airmeet Webhooks API](https://apis.io/apis/airmeet/airmeet-webhooks-api/) — Register webhook subscriptions for Airmeet event triggers.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Airmeet Webhooks](https://apis.io/asyncapis/airmeet/airmeet-webhooks-asyncapi/)

#### Event channels (21)

Individual events and webhooks the provider emits.

- [trigger.airmeet.attendee.added](https://apis.io/channels/airmeet/trigger-airmeet-attendee-added/)
- [trigger.airmeet.attendee.joined](https://apis.io/channels/airmeet/trigger-airmeet-attendee-joined/)
- [trigger.airmeet.created](https://apis.io/channels/airmeet/trigger-airmeet-created/)
- [trigger.airmeet.finished](https://apis.io/channels/airmeet/trigger-airmeet-finished/)
- [trigger.airmeet.polls](https://apis.io/channels/airmeet/trigger-airmeet-polls/)
- [trigger.airmeet.questions](https://apis.io/channels/airmeet/trigger-airmeet-questions/)
- [trigger.airmeet.registrant.added](https://apis.io/channels/airmeet/trigger-airmeet-registrant-added/)
- [trigger.airmeet.reminder](https://apis.io/channels/airmeet/trigger-airmeet-reminder/)
- [trigger.airmeet.started](https://apis.io/channels/airmeet/trigger-airmeet-started/)
- [trigger.attendee.booth.joined](https://apis.io/channels/airmeet/trigger-attendee-booth-joined/)
- [trigger.attendee.clicked_cta](https://apis.io/channels/airmeet/trigger-attendee-clicked-cta/)
- [trigger.attendee.engagement_score](https://apis.io/channels/airmeet/trigger-attendee-engagement-score/)
- [trigger.attendee.entered_airmeet](https://apis.io/channels/airmeet/trigger-attendee-entered-airmeet/)
- [trigger.attendee.joined_booth](https://apis.io/channels/airmeet/trigger-attendee-joined-booth/)
- [trigger.attendee.joined_session](https://apis.io/channels/airmeet/trigger-attendee-joined-session/)
- [trigger.attendee.joined_stage](https://apis.io/channels/airmeet/trigger-attendee-joined-stage/)
- [trigger.attendee.joined_table](https://apis.io/channels/airmeet/trigger-attendee-joined-table/)
- [trigger.attendee.ondemand_session_attendance](https://apis.io/channels/airmeet/trigger-attendee-ondemand-session-attendance/)
- [trigger.attendee.opened_resource](https://apis.io/channels/airmeet/trigger-attendee-opened-resource/)
- [trigger.leaderboard.scoreboard](https://apis.io/channels/airmeet/trigger-leaderboard-scoreboard/)
- [trigger.session.attendee.joined](https://apis.io/channels/airmeet/trigger-session-attendee-joined/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [airmeet](https://apis.io/servers/airmeet/airmeet/)

#### Collections (12)

Postman and Open Collection request collections.

- [Airmeet Public Authentication API](https://apis.io/collections/airmeet/open-airmeet-authentication-api/)
- [Airmeet Public Authentication Event Details API](https://apis.io/collections/airmeet/open-airmeet-event-details-api/)
- [Airmeet Public Authentication Manage Event API](https://apis.io/collections/airmeet/open-airmeet-manage-event-api/)
- [Airmeet Public Authentication Manage Event Series API](https://apis.io/collections/airmeet/open-airmeet-manage-event-series-api/)
- [Airmeet Public Authentication Manage Registrations API](https://apis.io/collections/airmeet/open-airmeet-manage-registrations-api/)
- [Airmeet Public Authentication Webhooks API](https://apis.io/collections/airmeet/open-airmeet-webhooks-api/)
- [Airmeet Public Authentication API](https://apis.io/collections/airmeet/postman-airmeet-authentication-api/)
- [Airmeet Public Authentication Event Details API](https://apis.io/collections/airmeet/postman-airmeet-event-details-api/)
- [Airmeet Public Authentication Manage Event API](https://apis.io/collections/airmeet/postman-airmeet-manage-event-api/)
- [Airmeet Public Authentication Manage Event Series API](https://apis.io/collections/airmeet/postman-airmeet-manage-event-series-api/)
- [Airmeet Public Authentication Manage Registrations API](https://apis.io/collections/airmeet/postman-airmeet-manage-registrations-api/)
- [Airmeet Public Authentication Webhooks API](https://apis.io/collections/airmeet/postman-airmeet-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Airmeet Openapi Overlay](https://apis.io/overlays/airmeet/airmeet-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Airmeet Authentication](https://apis.io/security/airmeet/airmeet-authentication/)
- [Airmeet Domain Security](https://apis.io/security/airmeet/airmeet-domain-security/)
- [Airmeet Trust Center](https://apis.io/security/airmeet/airmeet-trust-center/)
- [Airmeet Vulnerability Disclosure](https://apis.io/security/airmeet/airmeet-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.airmeet.com/)
- [Documentation](https://help.airmeet.com/support/home)
- [Getting started](https://help.airmeet.com/support/solutions/articles/82000467794-airmeet-public-api-introduction)
- [API reference](https://help.airmeet.com/support/solutions/articles/82000467794-airmeet-public-api-introduction)
- [Pricing](https://www.airmeet.com/hub/pricing/)
- [Sign up](https://www.airmeet.com/signup)
- [Support](https://help.airmeet.com/support/home)
- [Changelog](https://updates.airmeet.com/en/)
- [Blog](https://www.airmeet.com/hub/blog/)
- [Security](https://www.airmeet.com/hub/responsible-disclosure/)
- [Compliance](https://www.airmeet.com/hub/security-and-compliance/)
- [Trust centre](https://www.airmeet.com/hub/security-and-compliance/)
- [Terms of service](https://www.airmeet.com/hub/terms-of-use/)
- [Privacy policy](https://www.airmeet.com/hub/privacy-policy/)
- [Status](https://status.airmeet.com/)

## API Evangelist rating

**Kin Score 50.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 57.9 |
| Contract governance | 18.2 |
| Operational transparency | 34.2 |
| Developer ergonomics | 50.6 |
| Access clarity | 47.4 |

**Agent readiness 19.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/airmeet/](https://apis.io/providers/airmeet/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Airmeet: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/airmeet/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
