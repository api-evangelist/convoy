# Convoy

> The Cloud Native Webhooks Gateway — open-source plus managed Cloud.

[Convoy](https://getconvoy.io) is an open-source, cloud-native **webhooks gateway** for both sending and receiving webhooks. It positions itself as "the complete solution for secure, scalable, and reliable webhook delivery" and is used in production by Neynar, Spruce Health, Marble, Source.ag, Maple, Mono, Xendit, and others. This API Evangelist repository profiles the Convoy provider — its API surface, SDKs, OSS distribution, cloud pricing, rate-limit policy, and FinOps alignment.

The upstream Convoy project lives at [`github.com/frain-dev/convoy`](https://github.com/frain-dev/convoy) (Go, Elastic License v2.0, 2,805+ stars). The Convoy REST API spec itself is published under MPL 2.0.

## At a Glance

| Field | Value |
|---|---|
| Provider | Convoy (Frain Technologies) |
| Type | Company — OSS + managed Cloud |
| API style | REST, OpenAPI 3.0.0 |
| Spec version | 26.3.5 |
| Operations | 44 across 11 tags |
| Regions | US (`us.getconvoy.cloud`), EU (`eu.getconvoy.cloud`) |
| Authentication | Bearer API key in `Authorization` header |
| OSS license | Elastic License v2.0 |
| API spec license | Mozilla Public License 2.0 |
| Status page | <https://status.getconvoy.io> |
| Changelog | <https://getconvoy.io/changelog> |

## What's in this Repo

| Path | Purpose |
|---|---|
| [`apis.yml`](./apis.yml) | API Evangelist index of the Convoy API and all common provider properties. |
| [`openapi/convoy-openapi.yml`](./openapi/convoy-openapi.yml) | Title-cased copy of the Convoy OpenAPI 3.0.0 spec (44 paths, 123 schemas). |
| [`capabilities/`](./capabilities/) | 11 self-contained Naftiko capability files — one per OpenAPI tag. |
| [`json-schema/`](./json-schema/) | 8 standalone JSON Schemas for the core Convoy entities. |
| [`json-structure/`](./json-structure/) | 8 JSON Structure docs for the same entities. |
| [`json-ld/convoy-context.jsonld`](./json-ld/convoy-context.jsonld) | JSON-LD context aligning Convoy nouns with schema.org. |
| [`examples/`](./examples/) | 68 JSON examples: 8 entity examples + 60 operation examples. |
| [`rules/convoy-rules.yml`](./rules/convoy-rules.yml) | Spectral ruleset enforcing Convoy's API conventions. |
| [`vocabulary/convoy-vocabulary.yml`](./vocabulary/convoy-vocabulary.yml) | Operational + capability vocabulary for the Convoy domain. |
| [`plans/convoy-plans-pricing.yml`](./plans/convoy-plans-pricing.yml) | API Commons Plans 0.1 description of Self-Hosted, Pro, and Enterprise tiers. |
| [`rate-limits/convoy-rate-limits.yml`](./rate-limits/convoy-rate-limits.yml) | API Commons Rate Limits 0.1 — Pro cap, endpoint and subscription throttles, retry backoff. |
| [`finops/convoy-finops.yml`](./finops/convoy-finops.yml) | FOCUS-aligned FinOps mapping of the Convoy billing surface. |

## The Convoy API

Convoy exposes a single project-scoped REST API at `/v1/projects/{projectID}/...`. The OpenAPI spec lists **44 operations across 11 tags**:

| Tag | Operations | What it does |
|---|---:|---|
| Endpoints | 9 | Create / list / update / delete / activate / pause endpoints; roll signing secrets; test OAuth2. |
| Events | 8 | Ingest events; fan-out, broadcast, dynamic, replay, batch replay. |
| Subscriptions | 8 | Wire sources/filters to endpoints; test filter and transform functions. |
| Filters | 8 | Per-subscription header/body filter CRUD plus bulk + test. |
| Portal Links | 6 | Issue, refresh, and revoke embeddable customer-facing dashboard links. |
| Sources | 5 | Manage HTTP/REST/broker ingest sources; test verification function. |
| Event Types | 5 | Declare event types, import from OpenAPI, deprecate. |
| Event Deliveries | 5 | List/retrieve deliveries, batch retry, force resend, single retry. |
| Meta Events | 3 | Read and resend platform meta-events. |
| Delivery Attempts | 2 | List and retrieve raw HTTP attempts behind a delivery. |
| Onboard | 1 | Bootstrap project source + endpoint + subscription. |

Servers are split into two independently-deployed regions:

```
https://us.getconvoy.cloud/api    # US Region
https://eu.getconvoy.cloud/api    # EU Region
```

Authentication is a Bearer API key:

```
Authorization: Bearer {your_convoy_api_key}
```

## Core Capabilities

From the Convoy README and product docs:

- **Outbound and inbound webhooks** in one gateway.
- **HMAC signing** — simple and advanced (timestamp + versioned) formats, header `X-Convoy-Signature`, hex or base64 encoding, rolling secrets.
- **Retries** — linear (constant time) or **exponential backoff with jitter**: `min(delaySeconds * 2^attempt, maxRetrySeconds) + jitter`, default cap 7200s, default 20 attempts.
- **Fan-out routing** by event type or payload structure, with per-endpoint and per-subscription rate limits.
- **Message broker ingest** — Apache Kafka, Google Cloud Pub/Sub, AWS SQS, and RabbitMQ (AMQP).
- **Source providers** — GitHub, Shopify, Twitter/X, Mono, and generic HTTP with HMAC, Basic Auth, API Key, or custom JS verification.
- **OAuth2** (client credentials, JWT client assertion) and **mTLS** client certs for authenticated delivery.
- **Customer-facing portal links** — iframe-embeddable dashboards scoped to a subset of endpoints.
- **Observability** — Prometheus + Grafana dashboards published in [`frain-dev/prometheus-grafana-dashboard`](https://github.com/frain-dev/prometheus-grafana-dashboard).

## SDKs, CLI, and Tools

Convoy publishes official SDKs in **five languages** under the [frain-dev GitHub org](https://github.com/frain-dev):

| SDK | Repo |
|---|---|
| Go | [`convoy-go`](https://github.com/frain-dev/convoy-go) |
| JavaScript / TypeScript | [`convoy.js`](https://github.com/frain-dev/convoy.js) |
| Python | [`convoy-python`](https://github.com/frain-dev/convoy-python) |
| PHP | [`convoy-php`](https://github.com/frain-dev/convoy-php) |
| Ruby | [`convoy.rb`](https://github.com/frain-dev/convoy.rb) |

Plus:

- [`convoy-cli`](https://github.com/frain-dev/convoy-cli) — debug Convoy events locally.
- [`homebrew-tools`](https://github.com/frain-dev/homebrew-tools) — Homebrew formulas for Convoy binaries.
- [`helm-charts`](https://github.com/frain-dev/helm-charts) — Kubernetes Helm charts.
- [`convoy-ingester`](https://github.com/frain-dev/convoy-ingester) — serverless ingestion function.

## Naftiko Capabilities

One self-contained Naftiko capability file per OpenAPI tag. Each includes its own `consumes` block, REST exposer, and MCP exposer.

| File | Operations |
|---|---:|
| [`capabilities/convoy-endpoints.yaml`](./capabilities/convoy-endpoints.yaml) | 9 |
| [`capabilities/convoy-events.yaml`](./capabilities/convoy-events.yaml) | 8 |
| [`capabilities/convoy-subscriptions.yaml`](./capabilities/convoy-subscriptions.yaml) | 8 |
| [`capabilities/convoy-filters.yaml`](./capabilities/convoy-filters.yaml) | 8 |
| [`capabilities/convoy-portal-links.yaml`](./capabilities/convoy-portal-links.yaml) | 6 |
| [`capabilities/convoy-sources.yaml`](./capabilities/convoy-sources.yaml) | 5 |
| [`capabilities/convoy-event-types.yaml`](./capabilities/convoy-event-types.yaml) | 5 |
| [`capabilities/convoy-event-deliveries.yaml`](./capabilities/convoy-event-deliveries.yaml) | 5 |
| [`capabilities/convoy-meta-events.yaml`](./capabilities/convoy-meta-events.yaml) | 3 |
| [`capabilities/convoy-delivery-attempts.yaml`](./capabilities/convoy-delivery-attempts.yaml) | 2 |
| [`capabilities/convoy-onboard.yaml`](./capabilities/convoy-onboard.yaml) | 1 |

## Cloud Pricing (Reconciled to <https://getconvoy.io/pricing>)

| Plan | Price | Rate | Retention | SLA | Static IPs |
|---|---|---|---|---|---|
| **Self-Hosted** | $0 (Elastic License v2.0) | configurable | configurable | self-managed | self-managed |
| **Pro** | $99 / month | 25 events/sec | 7 days | 99.99% | $100/mo add-on |
| **Enterprise** | custom | custom | custom | 99.999% | included |

Enterprise adds SAML SSO, SOC 2, VPC peering and private networking, response-time SLA, and solutions engineering. See [`plans/convoy-plans-pricing.yml`](./plans/convoy-plans-pricing.yml) for the API-Commons-formatted artifact.

## Positioning

Among modern webhook-infrastructure providers, Convoy occupies an unusually broad slice:

- **Versus Svix** — both target outbound webhook sending with signing, retries, and portals, but Convoy is the only one of the two that is open-source under a permissive(-ish) Elastic License v2.0 and that also handles inbound webhooks.
- **Versus Hookdeck** — both handle inbound ingestion with broker fan-out, but Convoy bundles outbound delivery into the same gateway, and offers an OSS distribution.
- **Versus rolling-your-own** — Convoy ships the parts most teams build poorly: HMAC schemes (advanced with timestamps), retry backoff with jitter, circuit breaking, portal links, and broker bridges.

## Sources

Every claim in this profile traces back to a fetched URL:

- <https://getconvoy.io>
- <https://getconvoy.io/docs/>
- <https://getconvoy.io/docs/api-reference/welcome>
- <https://getconvoy.io/docs/api-reference/authentication>
- <https://getconvoy.io/docs/product-manual/signatures>
- <https://getconvoy.io/docs/product-manual/sources>
- <https://getconvoy.io/docs/webhook-guides/webhook-retries>
- <https://getconvoy.io/pricing>
- <https://getconvoy.io/changelog>
- <https://status.getconvoy.io>
- <https://github.com/frain-dev>
- <https://github.com/frain-dev/convoy>
- <https://raw.githubusercontent.com/frain-dev/convoy/main/docs/v3/openapi3.json>

---

Maintained as part of the [API Evangelist Network](https://github.com/api-evangelist). Last regenerated 2026-05-22 via the API Evangelist `run-pipeline` skill.
