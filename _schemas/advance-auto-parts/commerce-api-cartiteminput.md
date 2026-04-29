---
description: Request to add an item to the cart.
layout: schema
name: CartItemInput
properties_list:
- description: Product SKU to add.
  name: productId
  type: string
- description: Quantity to add.
  name: quantity
  type: integer
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-cartiteminput-schema.json
slug: commerce-api-cartiteminput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartItemInput\",\n  \"description\": \"Request to add an item to the cart.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"productId\",\n    \"quantity\"\n  ],\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product SKU to add.\",\n      \"example\": \"SKU-123456\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity to add.\",\n      \"example\": 2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-cartiteminput-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: CartItemInput
---
