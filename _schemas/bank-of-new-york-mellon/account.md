---
description: A BNY Mellon treasury account
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: Account number (masked)
  name: accountNumber
  type: string
- description: Account name
  name: accountName
  type: string
- description: Account type
  name: accountType
  type: string
- description: Account currency (ISO 4217)
  name: currency
  type: string
- description: Account status
  name: status
  type: string
- description: BNY Mellon bank code
  name: bankCode
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/account-schema.json
slug: account
source_filename: account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/account-schema.json\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"A BNY Mellon treasury account\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Account number (masked)\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account name\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Account type\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency (ISO 4217)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status\",\n      \"enum\": [\n        \"active\",\n      \
  \  \"inactive\",\n        \"closed\"\n      ]\n    },\n    \"bankCode\": {\n      \"type\": \"string\",\n      \"description\": \"BNY Mellon bank code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/account-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: Account
---
