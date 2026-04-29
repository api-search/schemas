---
description: POSTransaction schema from Aramark Marko API
layout: schema
name: POSTransaction
properties_list:
- description: Transaction identifier
  name: transactionId
  type: string
- description: Location identifier
  name: locationId
  type: string
- description: Transaction amount in USD
  name: amount
  type: number
- description: Number of items in the transaction
  name: items
  type: integer
- description: Transaction timestamp (ISO 8601)
  name: timestamp
  type: string
- description: Payment method used
  name: paymentMethod
  type: string
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-pos-transaction-schema.json
slug: marko-api-pos-transaction
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction identifier\",\n      \"example\": \"TXN-001\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier\",\n      \"example\": \"LOC-001\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount in USD\",\n      \"example\": 12.5\n    },\n    \"items\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items in the transaction\",\n      \"example\": 2\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Transaction timestamp (ISO 8601)\",\n      \"example\": \"2026-04-19T12:30:00Z\"\n    },\n    \"paymentMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Payment method used\",\n      \"enum\": [\n        \"CREDIT\",\n        \"DEBIT\",\n        \"\
  CASH\",\n        \"MEAL_PLAN\",\n        \"MOBILE\"\n      ],\n      \"example\": \"MEAL_PLAN\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-pos-transaction-schema.json\",\n  \"title\": \"POSTransaction\",\n  \"description\": \"POSTransaction schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-pos-transaction-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: POSTransaction
---
