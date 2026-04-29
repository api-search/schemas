---
description: A shopping cart.
layout: schema
name: Cart
properties_list:
- description: Cart identifier.
  name: id
  type: string
- description: Items in the cart.
  name: items
  type: array
- description: Cart subtotal before tax.
  name: subtotal
  type: number
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-cart-schema.json
slug: commerce-api-cart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cart\",\n  \"description\": \"A shopping cart.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Cart identifier.\",\n      \"example\": \"cart-abc123\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Items in the cart.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CartItem\"\n      }\n    },\n    \"subtotal\": {\n      \"type\": \"number\",\n      \"description\": \"Cart subtotal before tax.\",\n      \"example\": 109.98\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-cart-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: Cart
---
