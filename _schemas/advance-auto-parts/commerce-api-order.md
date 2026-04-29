---
description: A placed order.
layout: schema
name: Order
properties_list:
- description: Order identifier.
  name: id
  type: string
- description: Current order status.
  name: status
  type: string
- description: Order total.
  name: total
  type: number
- description: Order creation timestamp.
  name: createdAt
  type: string
- description: Items in the order.
  name: items
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-order-schema.json
slug: commerce-api-order
source_filename: commerce-api-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"description\": \"A placed order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Order identifier.\",\n      \"example\": \"order-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status.\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"shipped\",\n        \"delivered\",\n        \"cancelled\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"number\",\n      \"description\": \"Order total.\",\n      \"example\": 109.98\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order creation timestamp.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Items in the order.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CartItem\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-order-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: Order
---
