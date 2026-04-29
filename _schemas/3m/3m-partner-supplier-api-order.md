---
description: A purchase order placed with 3M
layout: schema
name: Order
properties_list:
- description: Unique order identifier
  name: orderId
  type: string
- description: Current order status
  name: status
  type: string
- description: Order creation timestamp
  name: createdAt
  type: string
- description: Total order value
  name: totalAmount
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Line items in the order
  name: items
  type: array
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-order-schema.json
slug: 3m-partner-supplier-api-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"A purchase order placed with 3M\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier\",\n      \"example\": \"ORD-67890\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"shipped\",\n        \"delivered\",\n        \"cancelled\"\n      ],\n      \"example\": \"shipped\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order creation timestamp\",\n      \"example\": \"2025-03-15T10:30:00Z\"\n    },\n    \"totalAmount\": {\n      \"\
  type\": \"number\",\n      \"description\": \"Total order value\",\n      \"example\": 499.95\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items in the order\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OrderItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-order-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: Order
---
