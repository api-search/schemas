---
description: Schema for a BJ's Wholesale Club order
layout: schema
name: BJS Order
properties_list:
- description: ''
  name: orderId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: items
  type: array
- description: ''
  name: subtotal
  type: number
- description: ''
  name: tax
  type: number
- description: ''
  name: total
  type: number
- description: ''
  name: createdAt
  type: string
- description: ''
  name: estimatedDelivery
  type: string
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
schema_file: json-schema/bjs-order-schema.json
slug: bjs-order
source_filename: bjs-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/main/json-schema/bjs-order-schema.json\",\n  \"title\": \"BJS Order\",\n  \"description\": \"Schema for a BJ's Wholesale Club order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"confirmed\", \"processing\", \"shipped\", \"delivered\", \"cancelled\"]\n    },\n    \"membershipNumber\": {\n      \"type\": \"string\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"productId\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" },\n          \"quantity\": { \"type\": \"integer\" },\n          \"unitPrice\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"subtotal\": {\
  \ \"type\": \"number\" },\n    \"tax\": { \"type\": \"number\" },\n    \"total\": { \"type\": \"number\" },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"estimatedDelivery\": { \"type\": \"string\", \"format\": \"date\" }\n  },\n  \"required\": [\"orderId\", \"status\", \"membershipNumber\", \"items\", \"total\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/json-schema/bjs-order-schema.json
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
title: BJS Order
---
