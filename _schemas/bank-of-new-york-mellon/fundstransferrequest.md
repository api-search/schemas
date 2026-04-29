---
description: Funds transfer request between accounts
layout: schema
name: FundsTransferRequest
properties_list:
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: debitAccountId
  type: string
- description: ''
  name: creditAccountId
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: memo
  type: string
- description: ''
  name: clientReference
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/fundstransferrequest-schema.json
slug: fundstransferrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/fundstransferrequest-schema.json\",\n  \"title\": \"FundsTransferRequest\",\n  \"type\": \"object\",\n  \"description\": \"Funds transfer request between accounts\",\n  \"required\": [\n    \"amount\",\n    \"currency\",\n    \"debitAccountId\",\n    \"creditAccountId\"\n  ],\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\"\n    },\n    \"creditAccountId\": {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"memo\": {\n      \"type\": \"string\"\n    },\n    \"clientReference\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/fundstransferrequest-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: FundsTransferRequest
---
