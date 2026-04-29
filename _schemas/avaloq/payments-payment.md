---
description: Payment instruction details
layout: schema
name: Payment
properties_list:
- description: Payment ID
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: executionDate
  type: string
- description: ''
  name: valueDate
  type: string
- description: End-to-end transaction reference
  name: endToEndId
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/payments-payment-schema.json
slug: payments-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-schema.json\",\n  \"title\": \"Payment\",\n  \"description\": \"Payment instruction details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Payment ID\",\n      \"example\": \"PAY-001234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"COMPLETED\",\n        \"REJECTED\",\n        \"CANCELLED\"\n      ],\n      \"example\": \"COMPLETED\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 5000.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"EUR\"\n    },\n    \"executionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-04-20\"\n    },\n   \
  \ \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-04-20\"\n    },\n    \"endToEndId\": {\n      \"type\": \"string\",\n      \"description\": \"End-to-end transaction reference\",\n      \"example\": \"E2E-001234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/payments-payment-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Payment
---
