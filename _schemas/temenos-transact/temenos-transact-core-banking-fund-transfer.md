---
description: A fund transfer operation in Temenos Transact for moving funds between accounts, supporting internal transfers, domestic payments, and cross-border transactions.
layout: schema
name: FundTransfer
properties_list:
- description: Unique transfer identifier
  name: transferId
  type: string
- description: Source account identifier
  name: debitAccountId
  type: string
- description: Currency of the debit account
  name: debitCurrency
  type: string
- description: Destination account identifier
  name: creditAccountId
  type: string
- description: Currency of the credit account
  name: creditCurrency
  type: string
- description: Transfer amount
  name: amount
  type: number
- description: Amount credited (may differ due to exchange rate)
  name: creditAmount
  type: number
- description: Type of transfer
  name: transferType
  type: string
- description: Current transfer status
  name: status
  type: string
- description: Value date of the transfer
  name: valueDate
  type: string
- description: Actual execution date
  name: executionDate
  type: string
- description: Applied exchange rate for cross-currency transfers
  name: exchangeRate
  type: number
- description: Total charges applied
  name: chargesAmount
  type: number
- description: Currency of the charges
  name: chargesCurrency
  type: string
- description: Transfer description or purpose
  name: narrative
  type: string
- description: End-to-end reference for payment tracking
  name: endToEndReference
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-fund-transfer-schema.json
slug: temenos-transact-core-banking-fund-transfer
source_filename: temenos-transact-core-banking-fund-transfer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FundTransfer\",\n  \"type\": \"object\",\n  \"description\": \"A fund transfer operation in Temenos Transact for moving funds between accounts, supporting internal transfers, domestic payments, and cross-border transactions.\",\n  \"properties\": {\n    \"transferId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transfer identifier\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Source account identifier\"\n    },\n    \"debitCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the debit account\"\n    },\n    \"creditAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Destination account identifier\"\n    },\n    \"creditCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the credit account\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n    \
  \  \"description\": \"Transfer amount\"\n    },\n    \"creditAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount credited (may differ due to exchange rate)\"\n    },\n    \"transferType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of transfer\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current transfer status\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Value date of the transfer\"\n    },\n    \"executionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Actual execution date\"\n    },\n    \"exchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"Applied exchange rate for cross-currency transfers\"\n    },\n    \"chargesAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total charges applied\"\n    },\n    \"chargesCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the charges\"\n    },\n\
  \    \"narrative\": {\n      \"type\": \"string\",\n      \"description\": \"Transfer description or purpose\"\n    },\n    \"endToEndReference\": {\n      \"type\": \"string\",\n      \"description\": \"End-to-end reference for payment tracking\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-fund-transfer-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: FundTransfer
---
