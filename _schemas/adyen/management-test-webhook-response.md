---
description: TestWebhookResponse schema from Adyen API
layout: schema
name: TestWebhookResponse
properties_list:
- description: List with test results. Each test webhook we send has a list element with the result.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-test-webhook-response-schema.json
slug: management-test-webhook-response
source_filename: management-test-webhook-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-webhook-response-schema.json\",\n  \"title\": \"TestWebhookResponse\",\n  \"description\": \"TestWebhookResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List with test results. Each test webhook we send has a list element with the result.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TestOutput\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-webhook-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestWebhookResponse
---
