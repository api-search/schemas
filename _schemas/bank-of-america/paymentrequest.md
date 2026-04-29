---
description: Payment initiation request
layout: schema
name: PaymentRequest
properties_list:
- description: Payment type (ACH_CREDIT, WIRE, SWIFT, CHECK, RTP, etc.)
  name: paymentType
  type: string
- description: Payment amount
  name: amount
  type: number
- description: Payment currency (ISO 4217)
  name: currency
  type: string
- description: Account to debit
  name: debitAccountId
  type: string
- description: Requested value date (ISO 8601)
  name: valueDate
  type: string
- description: Client reference number
  name: reference
  type: string
- description: Payment memo or description
  name: memo
  type: string
- description: ''
  name: beneficiary
  type: object
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/paymentrequest-schema.json
slug: paymentrequest
source_filename: paymentrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/paymentrequest-schema.json\",\n  \"title\": \"PaymentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payment initiation request\",\n  \"required\": [\n    \"paymentType\",\n    \"amount\",\n    \"currency\",\n    \"debitAccountId\",\n    \"beneficiary\"\n  ],\n  \"properties\": {\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Payment type (ACH_CREDIT, WIRE, SWIFT, CHECK, RTP, etc.)\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Payment amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Payment currency (ISO 4217)\"\n    },\n    \"debitAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account to debit\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"date\",\n      \"description\": \"Requested value date (ISO 8601)\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Client reference number\"\n    },\n    \"memo\": {\n      \"type\": \"string\",\n      \"description\": \"Payment memo or description\"\n    },\n    \"beneficiary\": {\n      \"$ref\": \"#/components/schemas/Beneficiary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/paymentrequest-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: PaymentRequest
---
