# Auth0 (auth0)

Auth0 (now part of Okta) is a leading identity-as-a-service platform providing authentication and authorization for applications, APIs, and AI agents. It implements OpenID Connect, OAuth 2.0, SAML 2.0, WS-Federation, and SCIM, and exposes a Management API (OpenAPI 3.1, 221 paths, 2,567 schemas), an Authentication API, a My Account API, a My Organization API, FGA (Fine-Grained Authorization, OpenFGA / Zanzibar-based), and Auth0 for AI Agents — covering Token Vault, asynchronous authorization, Auth for MCP, and FGA for RAG.

**URL:** [https://auth0.com](https://auth0.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

AI Agents, Authentication, Authorization, FGA, Identity Management, MCP, OAuth, Okta, OpenID Connect, SAML, Security, SCIM

## Timestamps

- **Created:** 2024-04-14
- **Modified:** 2026-05-22

## APIs

### Auth0 Management API

Comprehensive administrative API for managing Auth0 tenants — users, clients, connections, organizations, actions, event streams, branding, logs, roles, resource servers, and more. Published as OpenAPI 3.1 (Beta) with 221 paths and 2,567 schemas.

- **Human URL:** [auth0.com/docs/api/management/v2](https://auth0.com/docs/api/management/v2)
- **OpenAPI:** [openapi/auth0-management-api-openapi.yml](openapi/auth0-management-api-openapi.yml)
- **OpenAPI Source:** [auth0.com/docs/api/management/openapi.json](https://auth0.com/docs/api/management/openapi.json)
- **Spectral Rules:** [rules/auth0-management-rules.yml](rules/auth0-management-rules.yml)

### Auth0 Authentication API

Authentication endpoints implementing OpenID Connect, OAuth 2.0, SAML 2.0, WS-Federation, and Passwordless flows. Covers `/authorize`, `/oauth/token` (including Token Exchange and Device Code), `/v2/logout`, `/samlp/*`, `/mfa/*`, `/passwordless/*`, `/userinfo`, and `/dbconnections/*`.

- **Human URL:** [auth0.com/docs/api/authentication](https://auth0.com/docs/api/authentication)
- **OpenAPI:** [openapi/auth0-authentication-api-openapi.yml](openapi/auth0-authentication-api-openapi.yml)
- **Spectral Rules:** [rules/auth0-authentication-rules.yml](rules/auth0-authentication-rules.yml)

### Auth0 My Account API

User self-service endpoints for managing authentication factors and account settings. Recently extended with ACR enforcement for sensitive scopes.

- **Human URL:** [auth0.com/docs/api/myaccount](https://auth0.com/docs/api/myaccount)

### Auth0 My Organization API

Organization-scoped endpoints for B2B customers to manage their own Organizations — IdP configuration, SCIM provisioning, and Home Realm Discovery.

- **Human URL:** [auth0.com/docs/api/myorganization](https://auth0.com/docs/api/myorganization)

### Auth0 FGA (Fine-Grained Authorization)

Hosted offering of OpenFGA — the CNCF authorization service inspired by Google's Zanzibar. Relationship-based access control via stores, authorization models, tuples, check, expand, list-objects, and list-users endpoints. Used for B2B hierarchical permissions and FGA for RAG in AI agent retrieval pipelines.

- **Human URL:** [docs.fga.dev](https://docs.fga.dev)
- **OpenAPI:** [openapi/auth0-fga-openapi.yml](openapi/auth0-fga-openapi.yml)
- **Spectral Rules:** [rules/auth0-fga-rules.yml](rules/auth0-fga-rules.yml)
- **Project:** [openfga.dev](https://openfga.dev)

### Auth0 for AI Agents

Identity and authorization product line for AI agents. Bundles Token Vault (delegated API credentials for Google/GitHub/Slack etc.), asynchronous authorization (human-in-the-loop), Fine-Grained Authorization for RAG, and Auth for MCP (Client ID Metadata Registration + On-Behalf-Of Token Exchange + Resource Parameter Compatibility Mode). **Generally available as of 2026.**

- **Product:** [auth0.com/ai](https://auth0.com/ai)
- **MCP Server:** [github.com/auth0/auth0-mcp-server](https://github.com/auth0/auth0-mcp-server)
- **Agent Skills:** [github.com/auth0/agent-skills](https://github.com/auth0/agent-skills) (27 skills, Claude Code / Cursor / Copilot / 40+ AI assistants)

## Common Properties

- [Website](https://auth0.com/)
- [Documentation](https://auth0.com/docs/)
- [Getting Started](https://auth0.com/docs/get-started)
- [Blog](https://auth0.com/blog/)
- [Sign Up](https://auth0.com/signup)
- [Pricing](https://auth0.com/pricing) — also [plans/auth0-plans-pricing.yml](plans/auth0-plans-pricing.yml)
- [Rate Limits](rate-limits/auth0-rate-limits.yml)
- [FinOps](finops/auth0-finops.yml)
- [GitHub Organization](https://github.com/auth0)
- [Status Page](https://status.auth0.com/)
- [Community](https://community.auth0.com/)
- [Support](https://support.auth0.com/)
- [Terms of Service](https://auth0.com/legal/tos)
- [Privacy Policy](https://auth0.com/privacy)
- [SDK Libraries](https://auth0.com/docs/libraries)
- [Changelog](https://auth0.com/changelog)
- [Auth0 for AI Agents](https://auth0.com/ai)
- [Vocabulary](vocabulary/auth0-vocabulary.yml)
- [JSON-LD Context](json-ld/auth0-context.jsonld)

## Artifacts

Machine-readable API specifications and capability artifacts.

### OpenAPI Specifications

- [Auth0 Management API](openapi/auth0-management-api-openapi.yml) — OpenAPI 3.1, 221 paths, 2,567 schemas
- [Auth0 Authentication API](openapi/auth0-authentication-api-openapi.yml) — OpenAPI 3.0, 28 paths
- [Auth0 FGA / OpenFGA](openapi/auth0-fga-openapi.yml) — Swagger 2.0, 20 paths

### Spectral Rulesets

- [auth0-management-rules.yml](rules/auth0-management-rules.yml)
- [auth0-authentication-rules.yml](rules/auth0-authentication-rules.yml)
- [auth0-fga-rules.yml](rules/auth0-fga-rules.yml)

### Naftiko Capabilities

68 capabilities total — 47 for the Management API (one per resource group: users, clients, connections, organizations, actions, event-streams, guardian, branding, custom-domains, log-streams, network-acls, keys, prompts, refresh-tokens, resource-servers, risk-assessments, roles, self-service-profiles, sessions, token-exchange-profiles, user-attribute-profiles, verifiable-credentials, and more), 20 for the Authentication API (authorize-user, oauth-token, oidc, saml, ws-federation, mfa, passwordless, sso, logout, etc.), and 1 for FGA.

See [`capabilities/`](capabilities/).

### JSON Schemas

17 schemas extracted from the Management API OpenAPI for core entities — User, Client, Connection, Organization, Role, Action, Tenant, ResourceServer, EventStream, Hook, Rule, Branding, RefreshToken, Session, Form, Flow, CustomDomain.

See [`json-schema/`](json-schema/).

### JSON Structures

12 structural descriptors — Auth0 core entities plus FGA tuple/model.

See [`json-structure/`](json-structure/).

### JSON-LD Context

- [auth0-context.jsonld](json-ld/auth0-context.jsonld) — semantics for Auth0 + OAuth + OIDC + SAML + SCIM + FGA + MCP.

### Examples

- [User Create](examples/auth0-user-create-example.json)
- [OAuth Token (Client Credentials)](examples/auth0-oauth-token-client-credentials-example.json)
- [Authorize (PKCE)](examples/auth0-authorize-pkce-example.json)
- [Organization Create](examples/auth0-organization-create-example.json)
- [FGA Check](examples/auth0-fga-check-example.json)
- [MCP Server Init](examples/auth0-mcp-server-init-example.json)

### Vocabulary

- [auth0-vocabulary.yml](vocabulary/auth0-vocabulary.yml) — domains: Authentication, Authorization, Tokens, Tenancy & Organizations, Pipelines & Extensibility, AI Agent Identity, Operations.

### Plans / Rate Limits / FinOps

- [plans/auth0-plans-pricing.yml](plans/auth0-plans-pricing.yml) — Free / Essentials / Professional / Enterprise (B2C & B2B) + Auth0 for AI Agents (+50%), M2M Tokens, Enterprise SSO, Enterprise MFA add-ons.
- [rate-limits/auth0-rate-limits.yml](rate-limits/auth0-rate-limits.yml) — Authentication API 100/200 RPS, Management API 2/15 RPS, MFA SMS 10/hr, brute-force 20/min, extensibility 250 concurrent (Public Cloud), Public Performance Burst.
- [finops/auth0-finops.yml](finops/auth0-finops.yml) — FOCUS 1.3 aligned, meters for MAUs, M2M tokens, enterprise connections, organizations, AI Agents add-on, Token Vault credentials, FGA tuples.

## Pricing Summary

| Tier | B2C | B2B | MAUs |
|---|---|---|---|
| Free | $0 | $0 | up to 25,000 |
| Essentials | $35/mo | $150/mo | from 500 |
| Professional | $240/mo | $800/mo | from 500 |
| Enterprise | contact sales | contact sales | custom |

**Add-ons:** Auth0 for AI Agents (+50% of base), M2M Tokens ($30–$1,200/mo), Enterprise SSO Connections ($100/mo each beyond included), Enterprise MFA ($100/mo on B2B Essentials).

## Rate Limits Summary

| API | Free | Paid |
|---|---|---|
| Authentication API | 100 RPS | 200 RPS |
| Management API | 2 RPS | 15 RPS |

MFA SMS: 10/hour per device. Brute-force: 20 attempts/minute per IP per account. Extensibility concurrency: 250 (Public Cloud).

## Use Cases

| Name | Description |
|------|-------------|
| Customer Identity | Add secure, scalable authentication to customer-facing web and mobile applications with social login and passwordless options. |
| Workforce Identity | Federate with enterprise IdPs for employee authentication with SSO, MFA, and SCIM provisioning. |
| B2B Identity | Provide multi-tenant identity for SaaS applications with per-customer organization management and custom login flows. |
| API Authorization | Secure REST and GraphQL APIs using OAuth 2.0 access tokens with audience and scope validation. |
| Machine-to-Machine Auth | Issue OAuth 2.0 client credentials tokens for service-to-service API authentication without user involvement. |
| AI Agent Identity | Dedicated agent identities; broker user-delegated tokens to third-party APIs via Token Vault; FGA on RAG retrieval. |
| MCP Server Authentication | Auth for MCP (GA) secures Model Context Protocol servers via Client ID Metadata Registration and On-Behalf-Of Token Exchange. |

## Integrations

| Name | Description |
|------|-------------|
| Okta | Auth0 is part of Okta, enabling combined workforce and customer identity capabilities. |
| Active Directory / LDAP | Connect on-premises AD/LDAP directories for enterprise user authentication. |
| Azure AD / Entra ID | Federate with Azure AD for Microsoft ecosystem authentication and SSO. |
| Salesforce | Use Auth0 as identity provider for Salesforce apps and customer communities. |
| AWS | Secure AWS API Gateway and Lambda with Auth0-issued JWTs; deliver Event Streams to EventBridge. |
| Twilio | Send OTP and MFA codes via Twilio SMS and voice. |
| Stripe | Auth0 is available in the Stripe Projects developer preview. |
| LangChain / LlamaIndex / Vercel AI SDK / Cloudflare Agents / Firebase Genkit | Auth0 for AI Agents SDKs and adapters. |
| Claude Code / Cursor / GitHub Copilot | 27 Auth0 Agent Skills work with 40+ Agent-Skills-compatible coding assistants. |

## Solutions

| Name | Description |
|------|-------------|
| Customer Identity Access Management | Comprehensive CIAM with self-service registration, social login, adaptive MFA. |
| Workforce Identity | Enterprise identity for employees with federation, MFA, and SSO. |
| B2B SaaS Identity | Multi-tenant identity for SaaS platforms requiring per-customer branding, SSO, and user management. |
| AI Agent Security | Agent identity, token vaulting, async authorization, FGA-powered RAG; "Most Innovative AI Infrastructure Security Solution 2026." |

## SDKs by Language

- **JavaScript / TypeScript:** `auth0-spa-js`, `auth0-react` (984★), `auth0.js` (1.1k★), `nextjs-auth0` (2,295★), `node-auth0`
- **Go:** `go-jwt-middleware` (1,203★)
- **Java:** `auth0-java` (319★)
- **Swift:** `Auth0.swift` (445★)
- **Kotlin / Android:** `Auth0.Android` (287★)
- **Ruby:** `ruby-auth0` (204★)
- **Python:** `auth0-python`
- **PHP:** `auth0-PHP`
- **.NET:** `auth0.net`
- **Terraform:** `terraform-provider-auth0` (213★)

GitHub org [`auth0`](https://github.com/auth0) hosts 336 public repos.

## AI / Agent Affordances

- **Auth0 for AI Agents** (GA): Token Vault, asynchronous authorization, FGA for RAG, Auth for MCP.
- **MCP Server:** [`auth0/auth0-mcp-server`](https://github.com/auth0/auth0-mcp-server) — official, TypeScript, MIT, 108★. Install via `npx @auth0/auth0-mcp-server init`. Exposes Applications, Resource Servers, Actions, Logs, Forms, Application Grants to Claude Desktop / Cursor / Windsurf / VS Code. Read-only mode and glob tool filtering supported.
- **Agent Skills:** [`auth0/agent-skills`](https://github.com/auth0/agent-skills) — 27 skills covering Quickstart Router, Migration (Firebase/Cognito/Supabase/Clerk), MFA, ACUL Screen Generator, every major frontend (React/Vue/Angular/Next/Nuxt/Ionic/Expo) and backend (Express/Flask/Fastify/Spring Boot/FastAPI/ASP.NET) framework.
- **FGA for AI:** FGA Permissions Index (Developer Preview) pre-calculates permission paths for AI retrieval; reduces enterprise RAG over-fetching.
- **Frameworks supported:** LangChain, LlamaIndex, Cloudflare Agents, Vercel AI SDK, Firebase Genkit.

## Recent Releases (Changelog Highlights)

- **2026-05-19** — Suspicious IP Throttling for Custom Token Exchange
- **2026-05-12** — Account API ACR Enforcement (EA)
- **2026-05-11** — Online Refresh Tokens (Beta)
- **2026-05-06** — **Auth for MCP — Generally Available**
- **2026-05-05** — Private Key JWT on Enterprise Connections
- **2026-04-30** — Event Streams GA; FGA Permissions Index in Developer Preview
- **2026-04-28** — Organization Discovery by Domain GA
- **2026-04-23** — Deploy CLI Dry Run GA
- **2026-04-14** — Multi-Resource Refresh Tokens GA

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
