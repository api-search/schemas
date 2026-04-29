---
description: List of orders.
layout: schema
name: OrderList
properties_list:
- description: Array of orders.
  name: orders
  type: array
- description: Total number of orders.
  name: total
  type: integer
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-orderlist-schema.json
slug: commerce-api-orderlist
source_filename: commerce-api-orderlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderList\",\n  \"description\": \"List of orders.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"description\": \"Array of orders.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Order\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of orders.\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-orderlist-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: OrderList
---
