---
description: Payment instruction request
layout: schema
name: PaymentRequest
properties_list:
- description: Source account ID
  name: debtorAccountId
  type: string
- description: Destination IBAN
  name: creditorIban
  type: string
- description: Beneficiary name
  name: creditorName
  type: string
- description: Payment amount
  name: amount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Payment reference
  name: remittanceInfo
  type: string
- description: ''
  name: paymentType
  type: string
- description: ''
  name: executionDate
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/payments-payment-request-schema.json
slug: payments-payment-request
source_filename: payments-payment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-request-schema.json\",\n  \"title\": \"PaymentRequest\",\n  \"description\": \"Payment instruction request\",\n  \"type\": \"object\",\n  \"required\": [\n    \"debtorAccountId\",\n    \"creditorIban\",\n    \"amount\",\n    \"currency\"\n  ],\n  \"properties\": {\n    \"debtorAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Source account ID\",\n      \"example\": \"ACC-001234\"\n    },\n    \"creditorIban\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IBAN\",\n      \"example\": \"DE89370400440532013000\"\n    },\n    \"creditorName\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary name\",\n      \"example\": \"Jane Smith\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Payment amount\",\n \
  \     \"example\": 5000.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"example\": \"EUR\"\n    },\n    \"remittanceInfo\": {\n      \"type\": \"string\",\n      \"description\": \"Payment reference\",\n      \"example\": \"Invoice 2025-001\"\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SEPA_CREDIT\",\n        \"SWIFT\",\n        \"DOMESTIC\",\n        \"INSTANT\"\n      ],\n      \"example\": \"SEPA_CREDIT\"\n    },\n    \"executionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-04-20\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-request-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: PaymentRequest
---
