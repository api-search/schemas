---
description: A financial account managed through Montran's payment infrastructure. Represents both physical bank accounts and virtual accounts, with support for ISO 20022 camt message structures for balance and statement reporting.
layout: schema
name: Montran Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: Type of account
  name: accountType
  type: string
- description: International Bank Account Number
  name: iban
  type: string
- description: Proprietary account number
  name: accountNumber
  type: string
- description: Account currency (ISO 4217)
  name: currency
  type: string
- description: Name of the account owner
  name: ownerName
  type: string
- description: Account name or description
  name: accountName
  type: string
- description: Account status
  name: status
  type: string
- description: Account-holding financial institution
  name: institution
  type: object
- description: Account balances aligned with ISO 20022 camt.052 BankToCustomerAccountReport
  name: balances
  type: array
- description: Virtual account specific properties (when accountType is virtual)
  name: virtualAccount
  type: object
- description: Account creation timestamp
  name: createdAt
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
provider_name: Montran
provider_slug: montran
schema_file: json-schema/montran-account-schema.json
slug: montran-account
source_filename: montran-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.montran.com/schemas/account.json\",\n  \"title\": \"Montran Account\",\n  \"description\": \"A financial account managed through Montran's payment infrastructure. Represents both physical bank accounts and virtual accounts, with support for ISO 20022 camt message structures for balance and statement reporting.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"accountId\",\n    \"currency\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of account\",\n      \"enum\": [\n        \"physical\",\n        \"virtual\",\n        \"virtual_iban\"\n      ]\n    },\n    \"iban\": {\n      \"type\": \"string\",\n      \"description\": \"International Bank Account Number\",\n      \"pattern\": \"^[A-Z]{2}[0-9]{2}[A-Z0-9]{4,30}$\"\
  \n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Proprietary account number\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"ownerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the account owner\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Account name or description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"closed\",\n        \"blocked\"\n      ]\n    },\n    \"institution\": {\n      \"type\": \"object\",\n      \"description\": \"Account-holding financial institution\",\n      \"properties\": {\n        \"bic\": {\n          \"type\": \"string\",\n          \"description\": \"Bank Identifier Code (SWIFT/BIC)\",\n          \"\
  pattern\": \"^[A-Z]{4}[A-Z]{2}[A-Z0-9]{2}([A-Z0-9]{3})?$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the financial institution\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"balances\": {\n      \"type\": \"array\",\n      \"description\": \"Account balances aligned with ISO 20022 camt.052 BankToCustomerAccountReport\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Balance type code\",\n            \"enum\": [\n              \"CLBD\",\n              \"ITBD\",\n              \"OPBD\",\n              \"PRCD\",\n              \"XPCD\",\n              \"ITAV\"\n            ]\n          },\n          \"amount\": {\n            \"type\": \"number\"\
  ,\n            \"description\": \"Balance amount\"\n          },\n          \"currency\": {\n            \"type\": \"string\",\n            \"description\": \"Balance currency\",\n            \"pattern\": \"^[A-Z]{3}$\"\n          },\n          \"creditDebitIndicator\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"CRDT\",\n              \"DBIT\"\n            ]\n          },\n          \"dateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Balance date and time\"\n          }\n        }\n      }\n    },\n    \"virtualAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Virtual account specific properties (when accountType is virtual)\",\n      \"properties\": {\n        \"physicalAccountId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the underlying physical bank account\"\n        },\n        \"virtualIban\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Associated virtual IBAN\"\n        },\n        \"purpose\": {\n          \"type\": \"string\",\n          \"description\": \"Purpose of the virtual account\",\n          \"enum\": [\n            \"GENERAL\",\n            \"POBO\",\n            \"COBO\",\n            \"ESCROW\",\n            \"IN_HOUSE_BANK\",\n            \"TREASURY\"\n          ]\n        },\n        \"parentVirtualAccountId\": {\n          \"type\": \"string\",\n          \"description\": \"Parent virtual account for hierarchical structures\"\n        },\n        \"autoAllocate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether incoming payments are auto-allocated\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update\
  \ timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/json-schema/montran-account-schema.json
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
title: Montran Account
---
