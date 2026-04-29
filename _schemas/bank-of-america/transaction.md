---
description: An account transaction record
layout: schema
name: Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Account the transaction belongs to
  name: accountId
  type: string
- description: Transaction type (debit, credit)
  name: type
  type: string
- description: Transaction amount
  name: amount
  type: number
- description: Transaction currency
  name: currency
  type: string
- description: Transaction description or memo
  name: description
  type: string
- description: Bank reference number
  name: referenceNumber
  type: string
- description: Value date of the transaction
  name: valueDate
  type: string
- description: Post date of the transaction
  name: postDate
  type: string
- description: Transaction status
  name: status
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/transaction-schema.json
slug: transaction
source_filename: transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"type\": \"object\",\n  \"description\": \"An account transaction record\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account the transaction belongs to\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type (debit, credit)\",\n      \"enum\": [\n        \"debit\",\n        \"credit\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Transaction amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction currency\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Transaction description or memo\"\n    },\n    \"referenceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Bank reference number\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Value date of the transaction\"\n    },\n    \"postDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Post date of the transaction\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/transaction-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Transaction
---
