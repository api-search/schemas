---
description: Request to create a new order.
layout: schema
name: OrderInput
properties_list:
- description: Cart to convert to an order.
  name: cartId
  type: string
- description: Store for pickup.
  name: storeId
  type: string
- description: Fulfillment type.
  name: fulfillmentType
  type: string
- description: Payment method identifier.
  name: paymentMethodId
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-orderinput-schema.json
slug: commerce-api-orderinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderInput\",\n  \"description\": \"Request to create a new order.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"cartId\",\n    \"fulfillmentType\"\n  ],\n  \"properties\": {\n    \"cartId\": {\n      \"type\": \"string\",\n      \"description\": \"Cart to convert to an order.\",\n      \"example\": \"cart-abc123\"\n    },\n    \"storeId\": {\n      \"type\": \"string\",\n      \"description\": \"Store for pickup.\"\n    },\n    \"fulfillmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Fulfillment type.\",\n      \"enum\": [\n        \"store-pickup\",\n        \"same-day-delivery\",\n        \"standard-shipping\"\n      ]\n    },\n    \"paymentMethodId\": {\n      \"type\": \"string\",\n      \"description\": \"Payment method identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-orderinput-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: OrderInput
---
