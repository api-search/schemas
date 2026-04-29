---
description: A banking account arrangement in Temenos Transact. Created through the Arrangement Architecture supporting current, savings, corporate, Islamic, non-resident, and minor account types.
layout: schema
name: Account
properties_list:
- description: Unique system-generated account identifier
  name: accountId
  type: string
- description: Display name of the account
  name: accountName
  type: string
- description: Identifier of the owning customer
  name: customerId
  type: string
- description: Name of the owning customer
  name: customerName
  type: string
- description: Product identifier from the arrangement architecture
  name: productId
  type: string
- description: Human-readable product name
  name: productName
  type: string
- description: Type of account
  name: accountType
  type: string
- description: Account currency in ISO 4217 format
  name: currency
  type: string
- description: Current account status
  name: status
  type: string
- description: Date the account was opened
  name: openingDate
  type: string
- description: Current working balance of the account
  name: workingBalance
  type: number
- description: Available balance including overdraft facility
  name: availableBalance
  type: number
- description: Identifier of the assigned account officer
  name: accountOfficerId
  type: integer
- description: Branch where the account is held
  name: branchId
  type: string
- description: International Bank Account Number
  name: iban
  type: string
- description: Bank Identifier Code (SWIFT code)
  name: bic
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-account-schema.json
slug: temenos-transact-core-banking-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"A banking account arrangement in Temenos Transact. Created through the Arrangement Architecture supporting current, savings, corporate, Islamic, non-resident, and minor account types.\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system-generated account identifier\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the account\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the owning customer\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the owning customer\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier from the arrangement architecture\"\n    },\n    \"productName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Human-readable product name\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of account\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency in ISO 4217 format\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current account status\"\n    },\n    \"openingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the account was opened\"\n    },\n    \"workingBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Current working balance of the account\"\n    },\n    \"availableBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Available balance including overdraft facility\"\n    },\n    \"accountOfficerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the assigned account officer\"\n    },\n    \"branchId\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Branch where the account is held\"\n    },\n    \"iban\": {\n      \"type\": \"string\",\n      \"description\": \"International Bank Account Number\"\n    },\n    \"bic\": {\n      \"type\": \"string\",\n      \"description\": \"Bank Identifier Code (SWIFT code)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-account-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Account
---
