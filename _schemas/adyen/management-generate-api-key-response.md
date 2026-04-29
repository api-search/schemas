---
description: GenerateApiKeyResponse schema from Adyen API
layout: schema
name: GenerateApiKeyResponse
properties_list:
- description: The generated API key.
  name: apiKey
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-generate-api-key-response-schema.json
slug: management-generate-api-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-api-key-response-schema.json\",\n  \"title\": \"GenerateApiKeyResponse\",\n  \"description\": \"GenerateApiKeyResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiKey\": {\n      \"description\": \"The generated API key.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"apiKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-api-key-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GenerateApiKeyResponse
---
