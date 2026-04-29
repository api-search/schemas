---
description: ExciseTransaction schema from Avalara API
layout: schema
name: ExciseTransaction
properties_list:
- description: ''
  name: transactionId
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: transactionType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: totalTax
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-transaction-schema.json
slug: excise-excise-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-transaction-schema.json\",\n  \"title\": \"ExciseTransaction\",\n  \"description\": \"ExciseTransaction schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Committed\",\n        \"Voided\"\n      ]\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"totalTax\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-transaction-schema.json
tags:
- Taxes
title: ExciseTransaction
---
