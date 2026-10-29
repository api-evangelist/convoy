# Convoy

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

Convoy is an open-source, cloud-native webhooks gateway used to securely ingest, persist, debug, deliver, and manage events. It positions itself as "the complete solution for secure, scalable, and reliable webhook delivery," covering both outbound (sending) and inbound (receiving) webhooks with retries, payload signing, fan-out, rate limiting, message broker ingestion, and customer-facing portals. Convoy is offered as a self-hosted open-source project (Elastic License v2.0, with the OpenAPI spec under MPL 2.0) and a fully managed cloud service in US and EU regions.

**Areas:** Webhook · Webhook Gateway · Event Delivery · Eventing · Messaging · Integration · API Infrastructure

## Convoy on APIs.io

Everything profiled for Convoy is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/convoy/](https://apis.io/providers/convoy/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Convoy Delivery Attempts API](https://apis.io/apis/convoy/convoy-delivery-attempts-api/) — Delivery Attempt related APIs
- [Convoy Endpoints API](https://apis.io/apis/convoy/convoy-endpoints-api/) — Endpoint related APIs
- [Convoy Event Deliveries API](https://apis.io/apis/convoy/convoy-event-deliveries-api/) — EventDelivery related APIs
- [Convoy Events API](https://apis.io/apis/convoy/convoy-events-api/) — Event related APIs
- [Convoy Filters API](https://apis.io/apis/convoy/convoy-filters-api/) — Filters related APIs
- [Convoy Meta Events API](https://apis.io/apis/convoy/convoy-meta-events-api/) — Meta Events related APIs
- [Convoy Onboard API](https://apis.io/apis/convoy/convoy-onboard-api/) — Onboard related APIs
- [Convoy Portal Links API](https://apis.io/apis/convoy/convoy-portal-links-api/) — Portal Links related APIs
- [Convoy Sources API](https://apis.io/apis/convoy/convoy-sources-api/) — Source related APIs
- [Convoy Subscriptions API](https://apis.io/apis/convoy/convoy-subscriptions-api/) — Subscription related APIs
- [Convoy Event Types API](https://apis.io/apis/convoy/convoy-event-types-api/) — Event Types related APIs

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (12)

Multi-step workflows that chain operations into a business task.

- [Convoy Attach Filter to Subscription](https://apis.io/arazzos/convoy/convoy-attach-filter-to-subscription-workflow/)
- [Convoy Batch Retry Failed Deliveries](https://apis.io/arazzos/convoy/convoy-batch-retry-failed-deliveries-workflow/)
- [Convoy Broadcast Event and Track](https://apis.io/arazzos/convoy/convoy-broadcast-event-and-track-workflow/)
- [Convoy Create Event and Trace Delivery](https://apis.io/arazzos/convoy/convoy-create-event-and-trace-delivery-workflow/)
- [Convoy Define Event Type and Subscribe](https://apis.io/arazzos/convoy/convoy-define-event-type-and-subscribe-workflow/)
- [Convoy Fan Out Event to Owner](https://apis.io/arazzos/convoy/convoy-fanout-event-to-owner-workflow/)
- [Convoy Force Resend Successful Deliveries](https://apis.io/arazzos/convoy/convoy-force-resend-deliveries-workflow/)
- [Convoy Inspect Delivery Attempts](https://apis.io/arazzos/convoy/convoy-inspect-delivery-attempts-workflow/)
- [Convoy Provision Endpoint and Subscription](https://apis.io/arazzos/convoy/convoy-provision-endpoint-subscription-workflow/)
- [Convoy Register Incoming Source](https://apis.io/arazzos/convoy/convoy-register-incoming-source-workflow/)
- [Convoy Replay Event](https://apis.io/arazzos/convoy/convoy-replay-event-workflow/)
- [Convoy Retry a Failed Delivery](https://apis.io/arazzos/convoy/convoy-retry-failed-delivery-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Convoy Agentic Access](https://apis.io/agentic-access/convoy/convoy-agentic-access/)

#### JSON Schema (8)

The data models the API reads and writes.

- [Convoy DeliveryAttempt](https://apis.io/schemas/convoy/convoy-delivery-attempt/)
- [Convoy Endpoint](https://apis.io/schemas/convoy/convoy-endpoint/)
- [Convoy Event](https://apis.io/schemas/convoy/convoy-event/)
- [Convoy EventDelivery](https://apis.io/schemas/convoy/convoy-event-delivery/)
- [Convoy EventType](https://apis.io/schemas/convoy/convoy-event-type/)
- [Convoy PortalLink](https://apis.io/schemas/convoy/convoy-portal-link/)
- [Convoy Source](https://apis.io/schemas/convoy/convoy-source/)
- [Convoy Subscription](https://apis.io/schemas/convoy/convoy-subscription/)

#### JSON Structure (8)

Data models expressed in JSON Structure.

- [Convoy Delivery Attempt Structure](https://apis.io/json-structure/convoy/convoy-delivery-attempt-structure/)
- [Convoy Endpoint Structure](https://apis.io/json-structure/convoy/convoy-endpoint-structure/)
- [Convoy Event Delivery Structure](https://apis.io/json-structure/convoy/convoy-event-delivery-structure/)
- [Convoy Event Structure](https://apis.io/json-structure/convoy/convoy-event-structure/)
- [Convoy Event Type Structure](https://apis.io/json-structure/convoy/convoy-event-type-structure/)
- [Convoy Portal Link Structure](https://apis.io/json-structure/convoy/convoy-portal-link-structure/)
- [Convoy Source Structure](https://apis.io/json-structure/convoy/convoy-source-structure/)
- [Convoy Subscription Structure](https://apis.io/json-structure/convoy/convoy-subscription-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Convoy Context](https://apis.io/jsonld/convoy/convoy-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Convoy Vocabulary](https://apis.io/vocabularies/convoy/convoy-vocabulary/)

#### Examples (68)

Example requests and responses.

- [Convoy Delivery Attempt Example](https://apis.io/examples/convoy/convoy-delivery-attempt-example/)
- [Convoy Endpoint Example](https://apis.io/examples/convoy/convoy-endpoint-example/)
- [Convoy Event Delivery Example](https://apis.io/examples/convoy/convoy-event-delivery-example/)
- [Convoy Event Example](https://apis.io/examples/convoy/convoy-event-example/)
- [Convoy Event Type Example](https://apis.io/examples/convoy/convoy-event-type-example/)
- [Convoy Op Activateendpoint Example](https://apis.io/examples/convoy/convoy-op-activateendpoint-example/)
- [Convoy Op Batchreplayevents Example](https://apis.io/examples/convoy/convoy-op-batchreplayevents-example/)
- [Convoy Op Batchretryeventdelivery Example](https://apis.io/examples/convoy/convoy-op-batchretryeventdelivery-example/)
- [Convoy Op Bulkcreatefilters Example](https://apis.io/examples/convoy/convoy-op-bulkcreatefilters-example/)
- [Convoy Op Bulkonboard Example](https://apis.io/examples/convoy/convoy-op-bulkonboard-example/)
- [Convoy Op Bulkupdatefilters Example](https://apis.io/examples/convoy/convoy-op-bulkupdatefilters-example/)
- [Convoy Op Createbroadcastevent Example](https://apis.io/examples/convoy/convoy-op-createbroadcastevent-example/)
- [Convoy Op Createdynamicevent Example](https://apis.io/examples/convoy/convoy-op-createdynamicevent-example/)
- [Convoy Op Createendpoint Example](https://apis.io/examples/convoy/convoy-op-createendpoint-example/)
- [Convoy Op Createendpointevent Example](https://apis.io/examples/convoy/convoy-op-createendpointevent-example/)
- [Convoy Op Createendpointfanoutevent Example](https://apis.io/examples/convoy/convoy-op-createendpointfanoutevent-example/)
- [Convoy Op Createeventtype Example](https://apis.io/examples/convoy/convoy-op-createeventtype-example/)
- [Convoy Op Createfilter Example](https://apis.io/examples/convoy/convoy-op-createfilter-example/)
- [Convoy Op Createportallink Example](https://apis.io/examples/convoy/convoy-op-createportallink-example/)
- [Convoy Op Createsource Example](https://apis.io/examples/convoy/convoy-op-createsource-example/)
- [Convoy Op Createsubscription Example](https://apis.io/examples/convoy/convoy-op-createsubscription-example/)
- [Convoy Op Deleteendpoint Example](https://apis.io/examples/convoy/convoy-op-deleteendpoint-example/)
- [Convoy Op Deletefilter Example](https://apis.io/examples/convoy/convoy-op-deletefilter-example/)
- [Convoy Op Deletesource Example](https://apis.io/examples/convoy/convoy-op-deletesource-example/)
- [Convoy Op Deletesubscription Example](https://apis.io/examples/convoy/convoy-op-deletesubscription-example/)
- …and 43 more published on APIs.io

#### Collections (13)

Postman and Open Collection request collections.

- [Convoy API Reference](https://apis.io/collections/convoy/open-convoy/)
- [Convoy API Reference Delivery Attempts API](https://apis.io/collections/convoy/open-convoy-delivery-attempts-api/)
- [Convoy API Reference Delivery Attempts Endpoints API](https://apis.io/collections/convoy/open-convoy-endpoints-api/)
- [Convoy API Reference Delivery Attempts Event Deliveries API](https://apis.io/collections/convoy/open-convoy-event-deliveries-api/)
- [Convoy API Reference Delivery Attempts Events API](https://apis.io/collections/convoy/open-convoy-events-api/)
- [Convoy API Reference Delivery Attempts EventTypes API](https://apis.io/collections/convoy/open-convoy-eventtypes-api/)
- [Convoy API Reference Delivery Attempts Filters API](https://apis.io/collections/convoy/open-convoy-filters-api/)
- [Convoy API Reference Delivery Attempts Meta Events API](https://apis.io/collections/convoy/open-convoy-meta-events-api/)
- [Convoy API Reference Delivery Attempts Onboard API](https://apis.io/collections/convoy/open-convoy-onboard-api/)
- [Convoy API Reference Delivery Attempts Portal Links API](https://apis.io/collections/convoy/open-convoy-portal-links-api/)
- [Convoy API Reference Delivery Attempts Sources API](https://apis.io/collections/convoy/open-convoy-sources-api/)
- [Convoy API Reference Delivery Attempts Subscriptions API](https://apis.io/collections/convoy/open-convoy-subscriptions-api/)
- [Convoy API Reference](https://apis.io/collections/convoy/postman-convoy/)

#### Overlays (11)

OpenAPI overlays, including conversational phrasing for each operation.

- [Convoy Delivery Attempts Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-delivery-attempts-api-phrasing-overlay/)
- [Convoy Endpoints Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-endpoints-api-phrasing-overlay/)
- [Convoy Event Deliveries Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-event-deliveries-api-phrasing-overlay/)
- [Convoy Event Types Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-event-types-api-phrasing-overlay/)
- [Convoy Events Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-events-api-phrasing-overlay/)
- [Convoy Filters Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-filters-api-phrasing-overlay/)
- [Convoy Meta Events Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-meta-events-api-phrasing-overlay/)
- [Convoy Onboard Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-onboard-api-phrasing-overlay/)
- [Convoy Portal Links Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-portal-links-api-phrasing-overlay/)
- [Convoy Sources Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-sources-api-phrasing-overlay/)
- [Convoy Subscriptions Api Phrasing Overlay](https://apis.io/overlays/convoy/convoy-subscriptions-api-phrasing-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Convoy — jsonschema rules](https://apis.io/rules/convoy/convoy-jsonschema-spectral-rules/)
- [Convoy API Rules](https://apis.io/rules/convoy/convoy-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Convoy Authentication](https://apis.io/security/convoy/convoy-authentication/)
- [Convoy Domain Security](https://apis.io/security/convoy/convoy-domain-security/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Convoy Plans Pricing](https://apis.io/plans/convoy/convoy-plans-pricing/)
- [Convoy Price Estimates](https://apis.io/plans/convoy/convoy-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Convoy Rate Limits](https://apis.io/rate-limits/convoy/convoy-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Convoy Finops](https://apis.io/finops/convoy/convoy-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.getconvoy.io/)
- [Documentation](https://getconvoy.io/docs/)
- [Getting started](https://getconvoy.io/docs/quickstart)
- [API reference](https://getconvoy.io/docs/api-reference/welcome)
- [Pricing](https://getconvoy.io/pricing)
- [Changelog](https://getconvoy.io/changelog)
- [Blog](https://getconvoy.io/blog)
- [Security](https://getconvoy.io/docs/product-manual/signatures)
- [Compliance](https://getconvoy.io/pricing)
- [GitHub](https://github.com/frain-dev)
- [Status](https://status.getconvoy.io)

## API Evangelist rating

**Kin Score 66.9** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 67.9 |
| Contract quality | 68.8 |
| Contract governance | 27.3 |
| Operational transparency | 65.8 |
| Developer ergonomics | 70.2 |
| Access clarity | 67.1 |

**Agent readiness 33.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | yes |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 25.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/convoy/](https://apis.io/providers/convoy/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Convoy: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/convoy/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
