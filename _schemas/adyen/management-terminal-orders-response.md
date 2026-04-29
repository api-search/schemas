---
description: TerminalOrdersResponse schema from Adyen API
layout: schema
name: TerminalOrdersResponse
properties_list:
- description: List of orders for payment terminal packages and parts.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-orders-response-schema.json
slug: management-terminal-orders-response
source_filename: management-terminal-orders-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-orders-response-schema.json\",\n  \"title\": \"TerminalOrdersResponse\",\n  \"description\": \"TerminalOrdersResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List of orders for payment terminal packages and parts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TerminalOrder\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-orders-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalOrdersResponse
---
