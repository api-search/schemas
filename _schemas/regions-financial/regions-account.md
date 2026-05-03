---
description: A Regions Bank customer account (FDX-compliant)
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: FDX account type classification
  name: accountType
  type: string
- description: Masked account number (last 4 digits visible)
  name: accountNumber
  type: string
- description: Customer-assigned account nickname
  name: nickname
  type: string
- description: Account status
  name: status
  type: string
- description: Account currency code (ISO 4217)
  name: currency
  type: string
- description: ''
  name: balance
  type: object
- description: Institution name (Regions Bank)
  name: institution
  type: string
provider_name: regions-financial
provider_slug: regions-financial
schema_file: json-schema/regions-account-schema.json
slug: regions-account
source_filename: regions-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regions-financial/json-schema/regions-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"A Regions Bank customer account (FDX-compliant)\",\n  \"type\": \"object\",\n  \"required\": [\"accountId\", \"accountType\", \"status\"],\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\"CHECKING\", \"SAVINGS\", \"CREDIT_CARD\", \"LOAN\", \"INVESTMENT\", \"MORTGAGE\"],\n      \"description\": \"FDX account type classification\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Masked account number (last 4 digits visible)\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-assigned account nickname\"\n    },\n    \"\
  status\": {\n      \"type\": \"string\",\n      \"enum\": [\"OPEN\", \"CLOSED\"],\n      \"description\": \"Account status\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"description\": \"Account currency code (ISO 4217)\"\n    },\n    \"balance\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"available\": { \"type\": \"number\", \"description\": \"Available balance\" },\n        \"current\": { \"type\": \"number\", \"description\": \"Current ledger balance\" },\n        \"limit\": { \"type\": \"number\", \"description\": \"Credit limit for credit accounts\" },\n        \"currency\": { \"type\": \"string\", \"default\": \"USD\" },\n        \"asOf\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    },\n    \"institution\": {\n      \"type\": \"string\",\n      \"description\": \"Institution name (Regions Bank)\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/json-schema/regions-account-schema.json
tags:
- Banking
- Financial Services
- Open Banking
- FDX
- Consumer Banking
- Wealth Management
- Fortune 500
title: Account
---
