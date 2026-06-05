# Auth0 (auth0)

Auth0 (now part of Okta) is a leading identity-as-a-service platform providing authentication and authorization for applications, APIs, and AI agents. It implements OpenID Connect, OAuth 2.0, SAML 2.0, WS-Federation, and SCIM, and exposes a Management API (OpenAPI 3.1, 221 paths, 2,567 schemas), an Authentication API, a My Account API, a My Organization API, FGA (Fine-Grained Authorization, OpenFGA / Zanzibar-based), and Auth0 for AI Agents — covering Token Vault, asynchronous authorization, Auth for MCP, and FGA for RAG.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- AI Agents
- Authentication
- Authorization
- FGA
- Identity Management
- MCP
- OAuth
- Okta
- OpenID Connect
- SAML
- Security
- SCIM

## Timestamps

- **Created:** 2024-04-14
- **Modified:** 2026-05-30

## APIs

### Auth0 Management API

Comprehensive administrative API for managing Auth0 tenants — users, clients, connections, organizations, actions, event streams, branding, logs, roles, resource servers, and more. Published as OpenAPI 3.1 (Beta) with 221 paths and 2,567 schemas. Requires Management API access tokens (Bearer JWT or OAuth 2.0 client credentials).

- **Human URL:** [https://auth0.com/docs/api/management/v2](https://auth0.com/docs/api/management/v2)
- **Base URL:** `https://your-tenant.auth0.com/api/v2`

#### Tags

- Authentication
- Identity
- Management
- User Management

#### Properties

- [Documentation](https://auth0.com/docs/api/management/v2)
- [API Reference](https://auth0.com/docs/api/management/v2)
- [Getting Started](https://auth0.com/docs/get-started)
- [Authentication](https://auth0.com/docs/secure/tokens)
- [OpenAPI](openapi/auth0-management-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/auth0-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Open A P I Source](https://auth0.com/docs/api/management/openapi.json)
- [AsyncAPI](asyncapi/auth0-log-streams-and-actions-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Spectral Rules](rules/auth0-management-rules.yml)

### Auth0 Authentication API

Authentication endpoints implementing OpenID Connect, OAuth 2.0, SAML 2.0, WS-Federation, and Passwordless. Covers /authorize, /oauth/token (including Token Exchange and Device Code), /v2/logout, /samlp/*, /mfa/*, /passwordless/*, /userinfo, and /dbconnections/*.

- **Human URL:** [https://auth0.com/docs/api/authentication](https://auth0.com/docs/api/authentication)
- **Base URL:** `https://your-tenant.auth0.com`

#### Tags

- Authentication
- OAuth
- OpenID Connect
- SAML
- WS-Federation
- Passwordless
- MFA

#### Properties

- [Documentation](https://auth0.com/docs/api/authentication)
- [API Reference](https://auth0.com/docs/api/authentication)
- [OpenAPI](openapi/auth0-authentication-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/auth0-authentication-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-authentication-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/auth0-authentication-rules.yml)

### Auth0 My Account API

User self-service endpoints for managing authentication factors and account settings. Recently extended with ACR enforcement for sensitive scopes.

- **Human URL:** [https://auth0.com/docs/api/myaccount](https://auth0.com/docs/api/myaccount)
- **Base URL:** `https://your-tenant.auth0.com`

#### Tags

- Account Management
- Authentication
- MFA
- Self-Service

#### Properties

- [Documentation](https://auth0.com/docs/api/myaccount)
- [Postman Collection](collections/auth0-authentication-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-authentication-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-fga.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-fga.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Auth0 My Organization API

Organization-scoped endpoints for B2B customers to manage their own Organizations — IdP configuration, SCIM provisioning, and Home Realm Discovery.

- **Human URL:** [https://auth0.com/docs/api/myorganization](https://auth0.com/docs/api/myorganization)
- **Base URL:** `https://your-tenant.auth0.com`

#### Tags

- Authentication
- B2B
- Identity
- Organizations
- SCIM

#### Properties

- [Documentation](https://auth0.com/docs/api/myorganization)
- [Postman Collection](collections/auth0-authentication-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-authentication-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-fga.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-fga.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Auth0 FGA (Fine-Grained Authorization)

Auth0 FGA is the hosted offering of OpenFGA, the CNCF authorization service inspired by Google's Zanzibar. Provides relationship-based access control via stores, authorization models, tuples, check, expand, list-objects, and list-users endpoints. Used for B2B hierarchical permissions and FGA for RAG in AI agent retrieval pipelines.

- **Human URL:** [https://docs.fga.dev](https://docs.fga.dev)
- **Base URL:** `https://api.{region}.fga.dev`

#### Tags

- Authorization
- FGA
- OpenFGA
- Zanzibar
- ReBAC

#### Properties

- [Documentation](https://docs.fga.dev)
- [OpenAPI](openapi/auth0-fga-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/auth0-fga.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-fga.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/auth0-fga-rules.yml)
- [Project](https://openfga.dev)
- [Repository](https://github.com/openfga/openfga)

### Auth0 for AI Agents

Identity and authorization product line for AI agents. Bundles Token Vault (delegated API credentials for Google/GitHub/Slack etc.), asynchronous authorization (human-in-the-loop), Fine-Grained Authorization for RAG, and Auth for MCP (Client ID Metadata Registration + On-Behalf-Of Token Exchange + Resource Parameter Compatibility Mode). GA as of 2026.

- **Human URL:** [https://auth0.com/ai](https://auth0.com/ai)

#### Tags

- AI Agents
- MCP
- Token Vault
- GenAI
- RAG

#### Properties

- [Documentation](https://auth0.com/ai)
- [M C P Server](https://github.com/auth0/auth0-mcp-server)
- [Agent Skill](https://github.com/auth0/agent-skills)
- [SDK](https://auth0.com/docs/libraries)
- [Postman Collection](collections/auth0-authentication-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-authentication-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-fga.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-fga.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/auth0-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/auth0-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/auth0)
- [Website](https://auth0.com/)
- [Documentation](https://auth0.com/docs/)
- [Getting Started](https://auth0.com/docs/get-started)
- [Blog](https://auth0.com/blog/)
- [Sign Up](https://auth0.com/signup)
- [Login](https://manage.auth0.com/)
- [Pricing](https://auth0.com/pricing)
- [Plans](plans/auth0-plans-pricing.yml)
- [Rate Limits](rate-limits/auth0-rate-limits.yml)
- [Fin Ops](finops/auth0-finops.yml)
- [GitHub Organization](https://github.com/auth0)
- [Status Page](https://status.auth0.com/)
- [Community](https://community.auth0.com/)
- [Support](https://support.auth0.com/)
- [Terms of Service](https://auth0.com/legal/tos)
- [Privacy Policy](https://auth0.com/privacy)
- [SDK](https://auth0.com/docs/libraries)
- [Changelog](https://auth0.com/changelog)
- [A I](https://auth0.com/ai)
- [M C P Server](https://github.com/auth0/auth0-mcp-server)
- [Agent Skill](https://github.com/auth0/agent-skills)
- [Vocabulary](vocabulary/auth0-vocabulary.yml)
- [JSON-LD](json-ld/auth0-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [S D K Languages](undefined)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
