---
name: epicdirectories-webhook-create-and-test
description: Create a new webhook for a directory and immediately fire a test ping to verify the URL.
api: openapi/epicdirectories-openapi.json
operations:
- WebhooksController_create
- WebhooksController_test
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/epicdirectories-openapi.json ; every operationId checked against the contract
---

# epicdirectories-webhook-create-and-test

Create a new webhook for a directory and immediately fire a test ping to verify the URL.

## Steps

1. 1. Call `WebhooksController_create` with the required request body fields for the webhook (e.g., url, events) and include the authentication header `x-api-key`.
2. 2. Call `WebhooksController_test` with the `webhookId` returned from the create call and include the authentication header `x-api-key`.

## Rules

- Authentication: provide the API key in the request header `x-api-key` (or use Bearer token).
