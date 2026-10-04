---
name: atlassian-create-project-and-list
description: Create a new project and then retrieve the list of all projects.
api: openapi/atlassian-projects-api-openapi.yml
operations:
- atlassianCreateproject
- atlassianGetallprojects
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/atlassian-projects-api-openapi.yml ; every operationId checked against the contract
---

# atlassian-create-project-and-list

Create a new project and then retrieve the list of all projects.

## Steps

1. 1. Call `atlassianCreateproject` with the required request body fields for the new project.
2. 2. Call `atlassianGetallprojects` to retrieve the updated collection of projects.

## Rules

- Auth: Include an `Authorization` header with a valid API key, OAuth2 token, or Basic credentials as defined in the provider's auth schemes.
- Idempotency: The `atlassianCreateproject` operation is not idempotent; avoid duplicate calls unless the request body includes a unique project key.
