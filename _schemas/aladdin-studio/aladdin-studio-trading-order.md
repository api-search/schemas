---
description: A trading order in the Aladdin system
layout: schema
name: Order
properties_list:
- description: Unique order identifier
  name: orderId
  type: string
- description: Portfolio identifier
  name: portfolioId
  type: string
- description: Security identifier
  name: securityId
  type: string
- description: Order side
  name: side
  type: string
- description: Order quantity in shares or units
  name: quantity
  type: number
- description: Quantity filled
  name: filledQuantity
  type: number
- description: Average execution price
  name: averagePrice
  type: number
- description: Order status
  name: status
  type: string
- description: Order type
  name: orderType
  type: string
- description: Order creation timestamp
  name: createdAt
  type: string
- description: Order fill timestamp
  name: filledAt
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-trading-order-schema.json
slug: aladdin-studio-trading-order
source_filename: aladdin-studio-trading-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"A trading order in the Aladdin system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier\",\n      \"example\": \"ORD-987654\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"securityId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Order side\",\n      \"enum\": [\n        \"buy\",\n        \"sell\"\n      ],\n      \"example\": \"buy\"\n    },\n    \"quantity\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Order quantity in shares or units\",\n      \"example\": 100\n    },\n    \"filledQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity filled\",\n      \"example\": 100\n    },\n    \"averagePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Average execution price\",\n      \"example\": 195.0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order status\",\n      \"enum\": [\n        \"pending\",\n        \"filled\",\n        \"partially_filled\",\n        \"cancelled\"\n      ],\n      \"example\": \"filled\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"description\": \"Order type\",\n      \"enum\": [\n        \"market\",\n        \"limit\",\n        \"stop\"\n      ],\n      \"example\": \"market\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order creation\
  \ timestamp\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    },\n    \"filledAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order fill timestamp\",\n      \"example\": \"2026-04-19T10:31:05Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Order
---
