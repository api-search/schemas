---
description: A financial transaction record in Temenos Transact representing a debit or credit entry against an account.
layout: schema
name: Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Account against which the transaction was posted
  name: accountId
  type: string
- description: Type classification of the transaction
  name: transactionType
  type: string
- description: Whether the transaction is a debit or credit
  name: debitOrCredit
  type: string
- description: Transaction amount in account currency
  name: amount
  type: number
- description: Currency of the transaction
  name: currency
  type: string
- description: Date the transaction was booked
  name: bookingDate
  type: string
- description: Value date for interest calculation purposes
  name: valueDate
  type: string
- description: Date the transaction was processed
  name: processingDate
  type: string
- description: Transaction reference number
  name: reference
  type: string
- description: Transaction description or narrative text
  name: narrative
  type: string
- description: Account identifier of the counterparty
  name: counterpartyAccountId
  type: string
- description: Name of the counterparty
  name: counterpartyName
  type: string
- description: Running balance after this transaction
  name: balance
  type: number
- description: Exchange rate applied if currency conversion occurred
  name: exchangeRate
  type: number
- description: Charges applied to this transaction
  name: chargesAmount
  type: number
- description: Whether this transaction is a reversal
  name: reversalIndicator
  type: boolean
- description: Statement number this transaction belongs to
  name: statementNumber
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-transaction-schema.json
slug: temenos-transact-core-banking-transaction
source_filename: temenos-transact-core-banking-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Transaction\",\n  \"type\": \"object\",\n  \"description\": \"A financial transaction record in Temenos Transact representing a debit or credit entry against an account.\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account against which the transaction was posted\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the transaction\"\n    },\n    \"debitOrCredit\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the transaction is a debit or credit\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount in account currency\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Currency of the transaction\"\n    },\n    \"bookingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the transaction was booked\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Value date for interest calculation purposes\"\n    },\n    \"processingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the transaction was processed\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction reference number\"\n    },\n    \"narrative\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description or narrative text\"\n    },\n    \"counterpartyAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account identifier of the counterparty\"\n    },\n    \"counterpartyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the counterparty\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"\
  Running balance after this transaction\"\n    },\n    \"exchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"Exchange rate applied if currency conversion occurred\"\n    },\n    \"chargesAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Charges applied to this transaction\"\n    },\n    \"reversalIndicator\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this transaction is a reversal\"\n    },\n    \"statementNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Statement number this transaction belongs to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-transaction-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Transaction
---
