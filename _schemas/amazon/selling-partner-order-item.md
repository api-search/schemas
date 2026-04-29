---
description: OrderItem schema from Amazon Selling Partner API
layout: schema
name: OrderItem
properties_list:
- description: ''
  name: ASIN
  type: string
- description: ''
  name: OrderItemId
  type: string
- description: ''
  name: SellerSKU
  type: string
- description: ''
  name: Title
  type: string
- description: ''
  name: QuantityOrdered
  type: integer
- description: ''
  name: QuantityShipped
  type: integer
- description: ''
  name: ItemPrice
  type: object
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-order-item-schema.json
slug: selling-partner-order-item
source_filename: selling-partner-order-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ASIN\": {\n      \"type\": \"string\"\n    },\n    \"OrderItemId\": {\n      \"type\": \"string\"\n    },\n    \"SellerSKU\": {\n      \"type\": \"string\"\n    },\n    \"Title\": {\n      \"type\": \"string\"\n    },\n    \"QuantityOrdered\": {\n      \"type\": \"integer\"\n    },\n    \"QuantityShipped\": {\n      \"type\": \"integer\"\n    },\n    \"ItemPrice\": {\n      \"$ref\": \"#/components/schemas/Money\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderItem\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-item-schema.json\",\n  \"description\": \"OrderItem schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-item-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: OrderItem
---
