---
name: atlassian-invite-and-assign-user
description: Invite a new user to an organization and assign them product and organization roles.
api: openapi/atlassian-users-api-openapi.yml
operations:
- inviteUsers
- grantUserAccess
- assignOrganizationRole
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/atlassian-users-api-openapi.yml ; every operationId checked against the contract
---

# atlassian-invite-and-assign-user

Invite a new user to an organization and assign them product and organization roles.

## Steps

1. 1. Call `inviteUsers` with body fields `email`, `displayName`, and optional `groupIds`.
2. 2. Call `grantUserAccess` with path parameters `orgId` and `userId` and body field `roleId` to give product access.
3. 3. Call `assignOrganizationRole` with path parameters `orgId` and `userId` and body field `roleId` to assign an organization‑level role.

## Rules

- Authentication: include an `Authorization` header using either the `api_key` (Bearer token) or `OAuth2` scheme.
- Idempotency: `inviteUsers` is not idempotent; avoid duplicate invites by checking existing users first.
- Errors: expect HTTP 4xx for invalid parameters or missing permissions, and HTTP 5xx for server errors.
