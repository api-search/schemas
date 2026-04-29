---
description: RevenueSnapshot schema from Aramark Marko API
layout: schema
name: RevenueSnapshot
properties_list:
- description: Profit center identifier
  name: profitCenterId
  type: string
- description: Revenue period (YYYY-MM)
  name: period
  type: string
- description: Total revenue for the period in USD
  name: totalRevenue
  type: number
- description: Number of transactions in the period
  name: transactionCount
  type: integer
- description: Average transaction value in USD
  name: averageTicket
  type: number
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-revenue-snapshot-schema.json
slug: marko-api-revenue-snapshot
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"profitCenterId\": {\n      \"type\": \"string\",\n      \"description\": \"Profit center identifier\",\n      \"example\": \"PC-001\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Revenue period (YYYY-MM)\",\n      \"example\": \"2026-04\"\n    },\n    \"totalRevenue\": {\n      \"type\": \"number\",\n      \"description\": \"Total revenue for the period in USD\",\n      \"example\": 125430.5\n    },\n    \"transactionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of transactions in the period\",\n      \"example\": 3215\n    },\n    \"averageTicket\": {\n      \"type\": \"number\",\n      \"description\": \"Average transaction value in USD\",\n      \"example\": 39.02\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-revenue-snapshot-schema.json\"\
  ,\n  \"title\": \"RevenueSnapshot\",\n  \"description\": \"RevenueSnapshot schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-revenue-snapshot-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: RevenueSnapshot
---
