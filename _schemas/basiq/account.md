---
description: ''
layout: schema
name: Account
properties_list:
- description: ''
  name: id
  type: string
- description: Account name
  name: name
  type: string
- description: Masked account number
  name: accountNo
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current balance
  name: balance
  type: number
- description: Available funds
  name: availableFunds
  type: number
- description: ''
  name: accountType
  type: string
- description: ''
  name: status
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/account.json
slug: account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/account.json\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name\"\n    },\n    \"accountNo\": {\n      \"type\": \"string\",\n      \"description\": \"Masked account number\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Current balance\"\n    },\n    \"availableFunds\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Available funds\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"transaction\",\n\
  \        \"savings\",\n        \"credit-card\",\n        \"mortgage\",\n        \"loan\",\n        \"investment\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"available\",\n        \"unavailable\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/account.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: Account
---
