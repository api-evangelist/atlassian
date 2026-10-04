---
name: atlassian-create-and-transition-issue
description: Create a new issue and immediately transition it to a desired status.
api: openapi/atlassian-issues-api-openapi.yml
operations:
- atlassianCreateissue
- atlassianDotransition
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/atlassian-issues-api-openapi.yml ; every operationId checked against the contract
---

# atlassian-create-and-transition-issue

Create a new issue and immediately transition it to a desired status.

## Steps

1. 1. Call `atlassianCreateissue` with the JSON request body containing the required issue fields (e.g., project, summary, issuetype) and the `Authorization` header.
2. 2. Call `atlassianDotransition` with the path parameter `{issueIdOrKey}` returned from the create call, a JSON body specifying the transition `id`, and the `Authorization` header.

## Rules

- Auth: Include an `Authorization` header (OAuth2, API key, Basic, Bearer, etc.) as defined by the provider.
- Idempotency: Not applicable for these operations.
- Pagination: Not applicable for these operations.
- Errors: Follow the provider's standard HTTP error responses (e.g., 4xx for client errors, 5xx for server errors).
