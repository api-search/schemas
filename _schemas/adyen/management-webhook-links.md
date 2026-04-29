---
description: WebhookLinks schema from Adyen API
layout: schema
name: WebhookLinks
properties_list:
- description: The company account that the webhook is configured for. Only present for company-level webhooks.
  name: company
  type: object
- description: Generate an HMAC key.
  name: generateHmac
  type: object
- description: The merchant account that the webhook is configured for. Only present for merchant-level webhooks.
  name: merchant
  type: object
- description: Link to the resource itself.
  name: self
  type: object
- description: Test the webhook setup.
  name: testWebhook
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhook-links-schema.json
slug: management-webhook-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhook-links-schema.json\",\n  \"title\": \"WebhookLinks\",\n  \"description\": \"WebhookLinks schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"company\": {\n      \"description\": \"The company account that the webhook is configured for. Only present for company-level webhooks.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"generateHmac\": {\n      \"description\": \"Generate an HMAC key.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"merchant\": {\n      \"description\": \"The merchant account that the webhook is configured for. Only present for merchant-level webhooks.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"self\": {\n      \"description\": \"Link to the resource itself.\",\n      \"\
  $ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"testWebhook\": {\n      \"description\": \"Test the webhook setup.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    }\n  },\n  \"required\": [\n    \"self\",\n    \"testWebhook\",\n    \"generateHmac\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhook-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WebhookLinks
---
