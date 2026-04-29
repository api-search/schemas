---
description: ''
layout: schema
name: BankAccount
properties_list:
- description: Bank account identifier
  name: bankAccountId
  type: integer
- description: Bank account name
  name: bankAccountName
  type: string
- description: Bank account number
  name: bankAccountNum
  type: string
- description: Bank identifier
  name: bankId
  type: integer
- description: Bank name
  name: bankName
  type: string
- description: Bank branch identifier
  name: branchId
  type: integer
- description: Branch name
  name: branchName
  type: string
- description: Account currency code
  name: currencyCode
  type: string
- description: Account type
  name: accountType
  type: string
- description: Account status
  name: status
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-bank-account-schema.json
slug: financial-services-bank-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BankAccount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bank account identifier\"\n    },\n    \"bankAccountName\": {\n      \"type\": \"string\",\n      \"description\": \"Bank account name\"\n    },\n    \"bankAccountNum\": {\n      \"type\": \"string\",\n      \"description\": \"Bank account number\"\n    },\n    \"bankId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bank identifier\"\n    },\n    \"bankName\": {\n      \"type\": \"string\",\n      \"description\": \"Bank name\"\n    },\n    \"branchId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bank branch identifier\"\n    },\n    \"branchName\": {\n      \"type\": \"string\",\n      \"description\": \"Branch name\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency\
  \ code\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Account type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-bank-account-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: BankAccount
---
