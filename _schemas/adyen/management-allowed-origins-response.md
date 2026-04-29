---
description: AllowedOriginsResponse schema from Adyen API
layout: schema
name: AllowedOriginsResponse
properties_list:
- description: List of allowed origins.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-allowed-origins-response-schema.json
slug: management-allowed-origins-response
source_filename: management-allowed-origins-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-allowed-origins-response-schema.json\",\n  \"title\": \"AllowedOriginsResponse\",\n  \"description\": \"AllowedOriginsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List of allowed origins.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AllowedOrigin\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-allowed-origins-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AllowedOriginsResponse
---
