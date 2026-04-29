---
description: ''
layout: schema
name: Transaction
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: Raw transaction description from bank
  name: description
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: balance
  type: number
- description: ''
  name: direction
  type: string
- description: Basiq transaction class (e.g., payment, transfer)
  name: class
  type: string
- description: ''
  name: subClass
  type: object
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: postDate
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/transaction.json
slug: transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/transaction.json\",\n  \"title\": \"Transaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"posted\",\n        \"pending\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Raw transaction description from bank\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"credit\",\n        \"debit\"\n      ]\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Basiq transaction class (e.g., payment, transfer)\"\
  \n    },\n    \"subClass\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"postDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/transaction.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: Transaction
---
