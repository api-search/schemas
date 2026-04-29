---
description: A Bank of America CashPro account
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: Masked account number
  name: accountNumber
  type: string
- description: Account display name
  name: accountName
  type: string
- description: Account type (checking, savings, etc.)
  name: accountType
  type: string
- description: Account currency (ISO 4217)
  name: currency
  type: string
- description: ABA routing number
  name: routingNumber
  type: string
- description: Account status
  name: status
  type: string
- description: Date the account was opened
  name: openDate
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/account-schema.json
slug: account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/account-schema.json\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"A Bank of America CashPro account\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Masked account number\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account display name\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Account type (checking, savings, etc.)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency (ISO 4217)\"\n    },\n    \"routingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ABA routing number\"\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"closed\"\n      ]\n    },\n    \"openDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the account was opened\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/account-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Account
---
