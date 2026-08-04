# emnify (emnify)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
