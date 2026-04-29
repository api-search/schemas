---
description: API error response.
layout: schema
name: ErrorResponse
properties_list:
- description: Error code.
  name: code
  type: string
- description: Error message.
  name: message
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-errorresponse-schema.json
slug: catalog-api-errorresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"API error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code.\",\n      \"example\": \"NOT_FOUND\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message.\",\n      \"example\": \"The requested resource was not found.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-errorresponse-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: ErrorResponse
---
