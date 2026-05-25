# emnify

Cloud-native global IoT cellular connectivity. emnify operates its own mobile core and "SuperNetwork" across 540+ mobile network operators in 190+ countries, supplying multi-form-factor SIMs, eUICC-enabled cards, and SGP.32 IoT eSIM / Consumer eSIM profiles to enterprise IoT deployments.

This repo profiles the emnify developer surface — REST API, GraphQL API, Data Streamer, SDKs, MCP documentation server, plans, rate limits, and FinOps — as part of [API Evangelist](https://apievangelist.com/).

## APIs

| API | Description |
|---|---|
| [emnify REST API](https://docs.emnify.com/developers) | Primary HTTP API. 200+ operations across 150+ paths covering SIMs, endpoints, eUICCs (SGP.32), SMS, events, service/tariff profiles, organizations, users, IP, operators, system, and callbacks. JWT-bearer auth (application token or user credentials). |
| [emnify GraphQL API](https://docs.emnify.com/developers/graphql) | Flexible single-request queries with the in-browser GraphiQL IDE. |
| [emnify Data Streamer](https://docs.emnify.com/developers/reference/data-streamer) | Outbound event and usage streaming to AWS S3, Kinesis, REST/webhook, Datadog, Salesforce, and Keen.io. SMS and API callbacks deliver MO SMS and event payloads to your infrastructure. |
| [emnify Documentation MCP Server](https://docs.emnify.com/_mcp/server) | Public MCP server exposing emnify product and developer documentation to Claude Code, Cursor, and other MCP clients. |

## Artifacts

| Type | Path |
|---|---|
| OpenAPI 3.1 (full REST surface) | [`openapi/emnify-api-openapi.yml`](openapi/emnify-api-openapi.yml) — 152 paths, 214 operations, 709 schemas assembled from the public emnify `llms-full.txt` feed |
| Spectral ruleset | [`rules/emnify-rules.yml`](rules/emnify-rules.yml) |
| JSON Schemas | [`json-schema/emnify-sim-schema.json`](json-schema/emnify-sim-schema.json), [`json-schema/emnify-endpoint-schema.json`](json-schema/emnify-endpoint-schema.json), [`json-schema/emnify-event-schema.json`](json-schema/emnify-event-schema.json) |
| JSON Structure | [`json-structure/emnify-sim-structure.json`](json-structure/emnify-sim-structure.json), [`json-structure/emnify-endpoint-structure.json`](json-structure/emnify-endpoint-structure.json) |
| JSON-LD context | [`json-ld/emnify-context.jsonld`](json-ld/emnify-context.jsonld) |
| Examples | [`examples/`](examples/) — authenticate, list endpoints, send SMS, list events |
| Vocabulary | [`vocabulary/emnify-vocabulary.yml`](vocabulary/emnify-vocabulary.yml) |
| Plans / Pricing (API Commons 0.1) | [`plans/emnify-plans-pricing.yml`](plans/emnify-plans-pricing.yml) |
| Rate Limits (API Commons 0.1) | [`rate-limits/emnify-rate-limits.yml`](rate-limits/emnify-rate-limits.yml) |
| FinOps (FOCUS 1.3 aligned) | [`finops/emnify-finops.yml`](finops/emnify-finops.yml) |

## Naftiko Capabilities

Seven business-grouped capabilities packaged as Naftiko consume/expose definitions in [`capabilities/`](capabilities/):

- `sim-management.yaml` — SIM lifecycle (list, register, activate, suspend)
- `endpoint-management.yaml` — Endpoint/device CRUD and bulk operations, connectivity reset
- `sms-messaging.yaml` — Send MT SMS, list MO/MT SMS, cancel buffered messages
- `euicc-management.yaml` — SGP.32 eSIM eUICC and profile operations
- `events-monitoring.yaml` — Events, endpoint events, usage stats
- `policies-and-profiles.yaml` — Service profiles and tariff profiles
- `data-streamer-callbacks.yaml` — API callbacks and SMS callbacks for outbound streaming

## Authentication

The emnify REST API uses short-lived JWTs:

1. POST `/api/v1/authenticate` with an `application_token` (M2M) or username/password (with optional MFA).
2. The response contains an `auth_token` (JWT, ~4 hours) and a `refresh_token`.
3. Send the JWT as `Authorization: Bearer <auth_token>` on subsequent calls.

Rate limits to remember:

- 2,000 requests per IP per 5-minute window
- 10 million requests per organization per month
- 100 authenticate calls per IP per 5 minutes (cache JWTs)
- 10 req/s sustained on most list/stats endpoints; 100 req/s on enhanced endpoints; 50 req/s on individual endpoint operations

## SDKs and Tools

- [Python SDK](https://github.com/emnify/emnify-sdk-python) — `pip install emnify-sdk` (Apache-2.0)
- [Java SDK](https://github.com/emnify/emnify-sdk-java) (Apache-2.0)
- [Grafana PCAP Extractor Plugin](https://github.com/emnify/grafana-pcapextractor-plugin)
- [Akamai Insights Grafana Datasource](https://github.com/emnify/akamai-insights-datasource)
- Public MCP documentation server at `https://docs.emnify.com/_mcp/server`

## Sources

- emnify website — <https://www.emnify.com>
- Developer documentation — <https://docs.emnify.com/developers>
- Full doc feed (used to assemble OpenAPI) — <https://docs.emnify.com/llms-full.txt>
- GitHub organization — <https://github.com/EMnify>
- Plans and packages — <https://www.emnify.com/plans-and-packages>

## License

Provider content references are attributed to emnify GmbH. Artifacts authored in this repository are released under the same terms as the rest of the api-evangelist catalog.
