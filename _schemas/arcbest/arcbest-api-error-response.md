---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: integer
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-error-response-schema.json
slug: arcbest-api-error-response
source_filename: arcbest-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"Unauthorized access\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code\",\n      \"example\": 401\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-error-response-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: ErrorResponse
---
