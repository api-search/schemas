---
description: GenerateHmacKeyResponse schema from Adyen API
layout: schema
name: GenerateHmacKeyResponse
properties_list:
- description: The HMAC key generated for this webhook.
  name: hmacKey
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-generate-hmac-key-response-schema.json
slug: management-generate-hmac-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-hmac-key-response-schema.json\",\n  \"title\": \"GenerateHmacKeyResponse\",\n  \"description\": \"GenerateHmacKeyResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hmacKey\": {\n      \"description\": \"The HMAC key generated for this webhook.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"hmacKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-hmac-key-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GenerateHmacKeyResponse
---
