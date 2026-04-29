---
description: Request body for creating a new trading order
layout: schema
name: OrderRequest
properties_list:
- description: Portfolio identifier
  name: portfolioId
  type: string
- description: Security identifier
  name: securityId
  type: string
- description: Order side
  name: side
  type: string
- description: Order quantity
  name: quantity
  type: number
- description: Order type
  name: orderType
  type: string
- description: Limit price (required for limit orders)
  name: limitPrice
  type: number
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-trading-order-request-schema.json
slug: aladdin-studio-trading-order-request
source_filename: aladdin-studio-trading-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-request-schema.json\",\n  \"title\": \"OrderRequest\",\n  \"description\": \"Request body for creating a new trading order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"securityId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Order side\",\n      \"enum\": [\n        \"buy\",\n        \"sell\"\n      ],\n      \"example\": \"buy\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Order quantity\",\n      \"example\": 100\n    },\n    \"orderType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Order type\",\n      \"enum\": [\n        \"market\",\n        \"limit\",\n        \"stop\"\n      ],\n      \"example\": \"market\"\n    },\n    \"limitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Limit price (required for limit orders)\",\n      \"example\": 195.0\n    }\n  },\n  \"required\": [\n    \"portfolioId\",\n    \"securityId\",\n    \"side\",\n    \"quantity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-trading-order-request-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: OrderRequest
---
