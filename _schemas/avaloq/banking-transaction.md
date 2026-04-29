---
description: Bank account transaction
layout: schema
name: Transaction
properties_list:
- description: Transaction ID
  name: id
  type: string
- description: ''
  name: accountId
  type: string
- description: Transaction amount (positive=credit, negative=debit)
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: bookingDate
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: counterpartyName
  type: string
- description: ''
  name: counterpartyIban
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-transaction-schema.json
slug: banking-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Bank account transaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction ID\",\n      \"example\": \"TRX-001234\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"ACC-001234\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount (positive=credit, negative=debit)\",\n      \"example\": -1500.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"CHF\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-04-15\"\n    },\n    \"bookingDate\": {\n      \"type\": \"string\",\n     \
  \ \"format\": \"date\",\n      \"example\": \"2025-04-15\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Transfer to savings\"\n    },\n    \"counterpartyName\": {\n      \"type\": \"string\",\n      \"example\": \"Jane Smith\"\n    },\n    \"counterpartyIban\": {\n      \"type\": \"string\",\n      \"example\": \"DE89370400440532013000\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREDIT\",\n        \"DEBIT\",\n        \"FEE\",\n        \"INTEREST\"\n      ],\n      \"example\": \"DEBIT\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"BOOKED\",\n        \"CANCELLED\"\n      ],\n      \"example\": \"BOOKED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-transaction-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Transaction
---
