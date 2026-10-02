---
name: epicdirectories-payments-start-checkout
description: Start a checkout session for a premium listing boost after viewing available offers.
api: openapi/epicdirectories-openapi.json
operations:
- PaymentsController_offers
- PaymentsController_create
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/epicdirectories-openapi.json ; every operationId checked against the contract
---

# epicdirectories-payments-start-checkout

Start a checkout session for a premium listing boost after viewing available offers.

## Steps

1. 1. Retrieve the offers for the directory using `PaymentsController_offers` (path parameter `directory`).
2. 2. Initiate the checkout for the selected premium listing using `PaymentsController_create` (path parameters `directory`, `listingType`, `listingSlug`; request body as defined by the contract).

## Rules

- Include the API key in the `x-api-key` header for authentication.
- Use HTTPS endpoint `https://api.epicdirectories.com` for production calls.
