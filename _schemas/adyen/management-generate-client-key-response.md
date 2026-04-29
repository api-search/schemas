---
description: GenerateClientKeyResponse schema from Adyen API
layout: schema
name: GenerateClientKeyResponse
properties_list:
- description: Generated client key
  name: clientKey
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-generate-client-key-response-schema.json
slug: management-generate-client-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-client-key-response-schema.json\",\n  \"title\": \"GenerateClientKeyResponse\",\n  \"description\": \"GenerateClientKeyResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientKey\": {\n      \"description\": \"Generated client key\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"clientKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generate-client-key-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GenerateClientKeyResponse
---
