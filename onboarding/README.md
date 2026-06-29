# Programmatic API Onboarding — Atlassian

A single-file, zero-dependency Node.js (18+) CLI that reproduces SoundCloud's
`sc-api-auth.mjs` pattern for Atlassian: register an application / obtain credentials
programmatically instead of clicking through a dashboard, so agents and developers
can onboard at the command line.

- Script: [`atlassian-api-auth.mjs`](atlassian-api-auth.mjs)
- Run `node atlassian-api-auth.mjs --help` for usage and the required environment variables.
- Story / rationale: https://apievangelist.com/2026/08/29/atlassian-three-legged-oauth-console-first/

Part of the API Evangelist "Programmatic API Onboarding for the Agentic Moment" series.
