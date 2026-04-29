---
description: An item in the shopping cart.
layout: schema
name: CartItem
properties_list:
- description: Product SKU.
  name: productId
  type: string
- description: Quantity.
  name: quantity
  type: integer
- description: Price per unit.
  name: unitPrice
  type: number
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-cartitem-schema.json
slug: commerce-api-cartitem
source_filename: commerce-api-cartitem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartItem\",\n  \"description\": \"An item in the shopping cart.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product SKU.\",\n      \"example\": \"SKU-123456\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity.\",\n      \"example\": 2\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Price per unit.\",\n      \"example\": 54.99\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-cartitem-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: CartItem
---
