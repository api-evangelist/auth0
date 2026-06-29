# Programmatic API Onboarding — Auth0

A single-file, zero-dependency Node.js (18+) CLI that reproduces SoundCloud's
`sc-api-auth.mjs` pattern for Auth0: register an application / obtain credentials
programmatically instead of clicking through a dashboard, so agents and developers
can onboard at the command line.

- Script: [`auth0-api-auth.mjs`](auth0-api-auth.mjs)
- Run `node auth0-api-auth.mjs --help` for usage and the required environment variables.
- Story / rationale: https://apievangelist.com/2026/07/26/auth0-right-endpoint-still-asks-permission/

Part of the API Evangelist "Programmatic API Onboarding for the Agentic Moment" series.
