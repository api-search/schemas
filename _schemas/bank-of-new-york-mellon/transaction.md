---
description: A transaction on a BNY Mellon account
layout: schema
name: Transaction
properties_list:
- description: ''
  name: transactionId
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: debitCredit
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: referenceNumber
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: bookingDate
  type: string
- description: ''
  name: status
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/transaction-schema.json
slug: transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"type\": \"object\",\n  \"description\": \"A transaction on a BNY Mellon account\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"debitCredit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"debit\",\n        \"credit\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"referenceNumber\": {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"bookingDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/transaction-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: Transaction
---
