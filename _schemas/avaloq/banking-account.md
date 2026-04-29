---
description: Bank account details
layout: schema
name: Account
properties_list:
- description: Avaloq account ID
  name: id
  type: string
- description: IBAN or account number
  name: accountNumber
  type: string
- description: Account display name
  name: accountName
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current balance
  name: balance
  type: number
- description: Available balance after holds
  name: availableBalance
  type: number
- description: ''
  name: status
  type: string
- description: Owning customer ID
  name: customerId
  type: string
- description: ''
  name: openedDate
  type: string
- description: ''
  name: accountType
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-account-schema.json
slug: banking-account
source_filename: banking-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"Bank account details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Avaloq account ID\",\n      \"example\": \"ACC-001234\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"IBAN or account number\",\n      \"example\": \"CH56048350012345678009\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account display name\",\n      \"example\": \"Main Current Account\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"example\": \"CHF\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"Current\
  \ balance\",\n      \"example\": 250000.0\n    },\n    \"availableBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Available balance after holds\",\n      \"example\": 245000.0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"CLOSED\",\n        \"BLOCKED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Owning customer ID\",\n      \"example\": \"CUST-001234\"\n    },\n    \"openedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2020-01-15\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CURRENT\",\n        \"SAVINGS\",\n        \"INVESTMENT\",\n        \"CUSTODY\"\n      ],\n      \"example\": \"CURRENT\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-account-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Account
---
