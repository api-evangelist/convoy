# Convoy (convoy)

Convoy is an open-source, cloud-native webhooks gateway used to securely ingest, persist, debug, deliver, and manage events. It positions itself as "the complete solution for secure, scalable, and reliable webhook delivery," covering both outbound (sending) and inbound (receiving) webhooks with retries, payload signing, fan-out, rate limiting, message broker ingestion, and customer-facing portals. Convoy is offered as a self-hosted open-source project (Elastic License v2.0, with the OpenAPI spec under MPL 2.0) and a fully managed cloud service in US and EU regions.

**APIs.json:** [https://github.com/api-evangelist/convoy](https://github.com/api-evangelist/convoy)

## Scope

- **Type:** Index

## Tags

- Webhooks
- Webhook Gateway
- Event Delivery
- Eventing
- Messaging
- Integration
- API Infrastructure

## Timestamps

- **Created:** 2026-05-22
- **Modified:** 2026-05-22

## APIs

### Convoy API

The Convoy REST API, version 26.3.5, exposes 44 operations across 11 resource groups for managing webhook delivery infrastructure: Subscriptions, Endpoints, Events, Sources, Event Deliveries, Delivery Attempts, Portal Links, Meta Events, Event Types, Filters, and Onboard. All operations are scoped to a project (`/v1/projects/{projectID}/...`) and authenticated via Bearer API key in the Authorization header. The managed cloud is split into independently-deployed US and EU regions.

- **Human URL:** [https://getconvoy.io/docs/api-reference/welcome](https://getconvoy.io/docs/api-reference/welcome)
- **Base URL:** `https://us.getconvoy.cloud/api`

#### Tags

- Webhooks
- Event Delivery
- API Gateway
- Subscriptions
- Endpoints

#### Properties

- [OpenAPI](https://raw.githubusercontent.com/frain-dev/convoy/main/docs/v3/openapi3.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](./openapi/convoy-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/convoy.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/convoy.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://getconvoy.io/docs/api-reference/welcome)
- [Documentation](https://getconvoy.io/docs/)
- [Authentication](https://getconvoy.io/docs/api-reference/authentication)
- [Getting Started](https://getconvoy.io/docs/quickstart)
- [Regions](https://getconvoy.io/docs)
- [GitHub Repository](https://github.com/frain-dev/convoy)
- [Terms of Service](https://getconvoy.io/terms)
- [JSON Schema](./json-schema/convoy-endpoint-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-event-delivery-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-delivery-attempt-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-subscription-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-source-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-portal-link-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](./json-schema/convoy-event-type-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](./json-ld/convoy-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](./rules/convoy-rules.yml)
- [Vocabulary](./vocabulary/convoy-vocabulary.yml)
- [Examples](./examples/)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://getconvoy.io)
- [Developer Portal](https://getconvoy.io/docs/)
- [Documentation](https://getconvoy.io/docs/)
- [API Reference](https://getconvoy.io/docs/api-reference/welcome)
- [Getting Started](https://getconvoy.io/docs/quickstart)
- [Sign Up](https://dashboard.getconvoy.io/signup)
- [Login](https://dashboard.getconvoy.io/login)
- [Pricing](https://getconvoy.io/pricing)
- [Plans](./plans/convoy-plans-pricing.yml)
- [Rate Limits](./rate-limits/convoy-rate-limits.yml)
- [Changelog](https://getconvoy.io/changelog)
- [Blog](https://getconvoy.io/blog)
- [Status Page](https://status.getconvoy.io)
- [Security](https://getconvoy.io/docs/product-manual/signatures)
- [Compliance](https://getconvoy.io/pricing)
- [Support](mailto:support@getconvoy.io)
- [Contact](https://getconvoy.io)
- [GitHub Organization](https://github.com/frain-dev)
- [GitHub Repository](https://github.com/frain-dev/convoy)
- [SDK](https://github.com/frain-dev/convoy-go)
- [SDK](https://github.com/frain-dev/convoy.js)
- [SDK](https://github.com/frain-dev/convoy-python)
- [SDK](https://github.com/frain-dev/convoy-php)
- [SDK](https://github.com/frain-dev/convoy.rb)
- [C L I](https://github.com/frain-dev/convoy-cli)
- [C L I](https://github.com/frain-dev/homebrew-tools)
- [Integrations](https://github.com/frain-dev/helm-charts)
- [Integrations](https://github.com/frain-dev/prometheus-grafana-dashboard)
- [Integrations](https://github.com/frain-dev/convoy-ingester)
- [Code Examples](https://github.com/frain-dev/convoy-playground)
- [Code Examples](https://github.com/frain-dev/webhooks-with-kafka-demo)
- [Code Examples](https://github.com/frain-dev/convoy-paystack)
- [Features](undefined)
- [Features](undefined)
- [Features](undefined)
- [Regions](undefined)
- [Use Cases](undefined)
- [Customers](undefined)
- [L L Ms Txt](https://eu.getconvoy.cloud/llms.txt)
