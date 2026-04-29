---
description: A standing order instruction for recurring payments
layout: schema
name: StandingOrder
properties_list:
- description: Unique standing order identifier
  name: standingOrderId
  type: string
- description: Debit account identifier
  name: accountId
  type: string
- description: Beneficiary identifier
  name: beneficiaryId
  type: string
- description: Beneficiary account identifier
  name: beneficiaryAccountId
  type: string
- description: Name of the beneficiary
  name: beneficiaryName
  type: string
- description: Recurring payment amount
  name: amount
  type: number
- description: Payment currency
  name: currency
  type: string
- description: Payment frequency
  name: frequency
  type: string
- description: Date of the first payment
  name: startDate
  type: string
- description: Date of the last payment (optional for indefinite)
  name: endDate
  type: string
- description: Date of the next scheduled payment
  name: nextPaymentDate
  type: string
- description: Standing order status
  name: status
  type: string
- description: Payment description
  name: narrative
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-standing-order-schema.json
slug: temenos-transact-core-banking-standing-order
source_filename: temenos-transact-core-banking-standing-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StandingOrder\",\n  \"type\": \"object\",\n  \"description\": \"A standing order instruction for recurring payments\",\n  \"properties\": {\n    \"standingOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique standing order identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Debit account identifier\"\n    },\n    \"beneficiaryId\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary identifier\"\n    },\n    \"beneficiaryAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary account identifier\"\n    },\n    \"beneficiaryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the beneficiary\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Recurring payment amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Payment currency\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Payment frequency\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the first payment\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the last payment (optional for indefinite)\"\n    },\n    \"nextPaymentDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the next scheduled payment\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Standing order status\"\n    },\n    \"narrative\": {\n      \"type\": \"string\",\n      \"description\": \"Payment description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-standing-order-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: StandingOrder
---
