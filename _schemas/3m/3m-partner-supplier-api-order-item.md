---
description: A line item within an order
layout: schema
name: OrderItem
properties_list:
- description: Product identifier
  name: productId
  type: string
- description: Quantity ordered
  name: quantity
  type: integer
- description: Unit price at time of order
  name: unitPrice
  type: number
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-order-item-schema.json
slug: 3m-partner-supplier-api-order-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-item-schema.json\",\n  \"title\": \"OrderItem\",\n  \"description\": \"A line item within an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\",\n      \"example\": \"PROD-12345\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity ordered\",\n      \"example\": 20\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Unit price at time of order\",\n      \"example\": 24.99\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-item-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: OrderItem
---
