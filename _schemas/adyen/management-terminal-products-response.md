---
description: TerminalProductsResponse schema from Adyen API
layout: schema
name: TerminalProductsResponse
properties_list:
- description: Terminal products that can be ordered.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-products-response-schema.json
slug: management-terminal-products-response
source_filename: management-terminal-products-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-products-response-schema.json\",\n  \"title\": \"TerminalProductsResponse\",\n  \"description\": \"TerminalProductsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Terminal products that can be ordered.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TerminalProduct\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-products-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalProductsResponse
---
