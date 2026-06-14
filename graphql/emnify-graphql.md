# emnify GraphQL API

emnify provides a GraphQL API alongside its REST API, enabling flexible single-request queries against the emnify IoT connectivity data model. Clients can select exactly the fields they need, traverse related resources in a single round-trip, and explore the schema interactively via the built-in GraphiQL IDE.

**Endpoint:** `https://cdn.emnify.net/graphql` (authenticated via JWT bearer token)

**Interactive IDE:** https://docs.emnify.com/developers/graphql/graphiql-ide

**Documentation:** https://docs.emnify.com/developers/graphql

**Authentication:** Same short-lived JWT bearer tokens used by the REST API, obtained via application tokens or user credentials.

## Key Capabilities

- Query SIM inventory, status, and lifecycle state in a single request
- Retrieve endpoint (device) details, connectivity status, and assigned service/tariff profiles
- Inspect data sessions, usage statistics, and quota configurations
- Explore network coverage, operator lists, and roaming profiles
- Manage organizations, users, API tokens, and webhook configurations
- Retrieve invoices, usage breakdowns, and billing summaries
- Configure alerts, MFA settings, and VPN/breakout configurations

## Schema File

See [emnify-schema.graphql](emnify-schema.graphql) for the full conceptual GraphQL schema covering 50+ named types across the emnify data model.

## References

- Documentation: https://docs.emnify.com/developers/graphql
- GraphiQL IDE: https://docs.emnify.com/developers/graphql/graphiql-ide
- API Guidelines: https://docs.emnify.com/developers/api-guidelines/conventions
- Authentication: https://docs.emnify.com/developers/auth/application-tokens
- REST API (companion): https://docs.emnify.com/developers
