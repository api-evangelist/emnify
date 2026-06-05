# emnify (emnify)

emnify is a cloud-native global IoT cellular connectivity provider operating its own mobile core and SuperNetwork across 540+ MNOs in 190+ countries. emnify supplies SIMs, eUICC-enabled multi-form-factor cards, and Consumer/Advanced eSIM (SGP.32) profiles to enterprise IoT deployments — fleet tracking, EV charging, point-of-sale, smart buildings, micromobility, airline crew tablets, and more. The emnify REST API, GraphQL API, and Data Streamer give programmatic control over SIMs, endpoints, service and tariff profiles, eUICC profile operations, events, SMS, callbacks, and outbound usage/event streaming to S3, Kinesis, and webhooks. NTN-IoT satellite connectivity via Skylo extends coverage beyond terrestrial cellular.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- IoT
- Internet of Things
- Cellular Connectivity
- IoT SIM
- eSIM
- Consumer eSIM
- SGP.32
- M2M
- NTN-IoT
- Satellite
- SuperNetwork

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### emnify REST API

The emnify REST API gives programmatic access to the emnify IoT SuperNetwork — global cellular connectivity for IoT devices. Manage SIMs, endpoints (devices), service and tariff profiles, events, SMS, eSIM (SGP.32) profiles, organizations, users, API callbacks, and the Data Streamer. Authenticate with short-lived JWTs obtained via application tokens or user credentials.

- **Human URL:** [https://docs.emnify.com/developers](https://docs.emnify.com/developers)

#### Tags

- IoT
- Cellular
- Connectivity
- SIM
- eSIM

#### Properties

- [Documentation](https://docs.emnify.com/developers)
- [Documentation](https://docs.emnify.com/developers/api-guidelines/conventions)
- [Documentation](https://docs.emnify.com/llms-full.txt)
- [OpenAPI](openapi/emnify-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/emnify-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/emnify-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/emnify-rules.yml)
- [JSON Schema](json-schema/emnify-sim-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/emnify-endpoint-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/emnify-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/emnify-sim-structure.json)
- [JSON Structure](json-structure/emnify-endpoint-structure.json)
- [JSON-LD](json-ld/emnify-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/emnify-authenticate-example.json)
- [Example](examples/emnify-list-endpoints-example.json)
- [Example](examples/emnify-send-sms-example.json)
- [Example](examples/emnify-list-events-example.json)
- [Vocabulary](vocabulary/emnify-vocabulary.yml)

### emnify GraphQL API

emnify GraphQL API for flexible, single-request queries against the emnify data model with customizable response shapes. An in-browser GraphiQL IDE supports interactive exploration and testing.

- **Human URL:** [https://docs.emnify.com/developers/graphql](https://docs.emnify.com/developers/graphql)

#### Tags

- IoT
- GraphQL
- Query

#### Properties

- [Documentation](https://docs.emnify.com/developers/graphql)
- [Documentation](https://docs.emnify.com/developers/graphql/graphiql-ide)
- [Documentation](https://docs.emnify.com/developers/api-guidelines/conventions)
- [Postman Collection](collections/emnify-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/emnify-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### emnify Data Streamer

Stream event and usage data to outbound destinations (AWS S3, AWS Kinesis, REST/webhook, Datadog, Salesforce, Keen.io). Supports detailed object schemas for data types, traffic types, tariffs, operators, and volume tracking. SMS and API callbacks deliver mobile-originated SMS and event payloads to your infrastructure.

- **Human URL:** [https://docs.emnify.com/developers/reference/data-streamer](https://docs.emnify.com/developers/reference/data-streamer)

#### Tags

- Streaming
- Events
- Data
- Webhooks

#### Properties

- [Documentation](https://docs.emnify.com/developers/reference/data-streamer)
- [Documentation](https://docs.emnify.com/developers/integrations/data-streamer/aws-s3-kinesis)
- [Documentation](https://docs.emnify.com/developers/callbacks/api)
- [Documentation](https://docs.emnify.com/developers/callbacks/sms)
- [Postman Collection](collections/emnify-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/emnify-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### emnify Documentation MCP Server

Public MCP server for emnify documentation. Connect Claude Code, Cursor, or any MCP-aware client to query emnify product, developer, and API reference content directly from your AI assistant.

- **Human URL:** [https://docs.emnify.com/_mcp/server](https://docs.emnify.com/_mcp/server)

#### Tags

- MCP
- Documentation
- AI

#### Properties

- [M C P](https://docs.emnify.com/_mcp/server)
- [Documentation](https://docs.emnify.com/developers/developer-tools/ai-assistance)
- [Postman Collection](collections/emnify-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/emnify-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.emnify.com)
- [Documentation](https://docs.emnify.com)
- [Documentation](https://docs.emnify.com/developers)
- [Getting Started](https://docs.emnify.com/quickstart)
- [Sign Up](https://www.emnify.com/get-started)
- [Pricing](https://www.emnify.com/plans-and-packages)
- [GitHub Organization](https://github.com/EMnify)
- [SDK](https://github.com/emnify/emnify-sdk-python)
- [SDK](https://github.com/emnify/emnify-sdk-java)
- [SDK](https://pypi.org/project/emnify-sdk/)
- [Documentation](https://emnify.github.io/emnify-sdk-python/autoapi/index.html)
- [Documentation](https://docs.emnify.com/developers/sdks)
- [Documentation](https://docs.emnify.com/developers/sdks/python/quickstart)
- [Documentation](https://docs.emnify.com/developers/sdks/java/quickstart)
- [Documentation](https://docs.emnify.com/developers/auth/application-tokens)
- [Documentation](https://docs.emnify.com/developers/auth/user-credentials)
- [Documentation](https://docs.emnify.com/developers/auth/multi-factor-authentication)
- [Documentation](https://docs.emnify.com/developers/auth/jwts)
- [Rate Limits](https://docs.emnify.com/developers/api-guidelines/rate-limits)
- [Errors](https://docs.emnify.com/developers/api-guidelines/errors)
- [Pagination](https://docs.emnify.com/developers/api-guidelines/collections-pagination)
- [Conventions](https://docs.emnify.com/developers/api-guidelines/conventions)
- [Changelog](https://docs.emnify.com/changelog)
- [Support](https://support.emnify.com/hc/en-us/requests/new)
- [Forum](https://www.emnify.com/iot-blog)
- [Blog](https://www.emnify.com/iot-blog)
- [Terms of Service](https://www.emnify.com/legal/terms-and-conditions)
- [Privacy Policy](https://www.emnify.com/legal/privacy-statement)
- [Trust Center](https://www.emnify.com/iot-security)
- [Tool](https://github.com/emnify/grafana-pcapextractor-plugin)
- [Tool](https://github.com/emnify/akamai-insights-datasource)
- [LinkedIn](https://www.linkedin.com/company/emnify)
- [Twitter](https://twitter.com/emnify)
- [YouTube](https://www.youtube.com/c/emnify)
- [Plans](plans/emnify-plans-pricing.yml)
- [Rate Limits](rate-limits/emnify-rate-limits.yml)
- [Fin Ops](finops/emnify-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
