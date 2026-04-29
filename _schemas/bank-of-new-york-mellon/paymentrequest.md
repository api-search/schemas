---
description: Payment initiation request
layout: schema
name: PaymentRequest
properties_list:
- description: Payment type (WIRE, ACH_CREDIT, ACH_DEBIT, SWIFT, CHIPS)
  name: paymentType
  type: string
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
  name: valueDate
  type: string
- description: ''
  name: creditorName
  type: string
- description: ''
  name: creditorAccountNumber
  type: string
- description: ''
  name: creditorBankCode
  type: string
- description: ''
  name: creditorSwiftCode
  type: string
- description: ''
  name: remittanceInfo
  type: string
- description: ''
  name: clientReference
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/paymentrequest-schema.json
slug: paymentrequest
source_filename: paymentrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/paymentrequest-schema.json\",\n  \"title\": \"PaymentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payment initiation request\",\n  \"required\": [\n    \"paymentType\",\n    \"amount\",\n    \"currency\",\n    \"debitAccountId\",\n    \"creditorName\",\n    \"creditorAccountNumber\"\n  ],\n  \"properties\": {\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Payment type (WIRE, ACH_CREDIT, ACH_DEBIT, SWIFT, CHIPS)\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"creditorName\": {\n      \"type\": \"string\"\n    },\n    \"creditorAccountNumber\"\
  : {\n      \"type\": \"string\"\n    },\n    \"creditorBankCode\": {\n      \"type\": \"string\"\n    },\n    \"creditorSwiftCode\": {\n      \"type\": \"string\"\n    },\n    \"remittanceInfo\": {\n      \"type\": \"string\"\n    },\n    \"clientReference\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/paymentrequest-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: PaymentRequest
---
