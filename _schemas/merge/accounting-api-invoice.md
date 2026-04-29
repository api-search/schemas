---
description: An invoice from a connected accounting system in the Merge Unified API.
layout: schema
name: Invoice
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: remote_id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: contact
  type: string
- description: Invoice number.
  name: number
  type: string
- description: ''
  name: issue_date
  type: string
- description: ''
  name: due_date
  type: string
- description: ''
  name: paid_on_date
  type: string
- description: ''
  name: memo
  type: string
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: ''
  name: total_discount
  type: number
- description: ''
  name: sub_total
  type: number
- description: ''
  name: total_tax_amount
  type: number
- description: ''
  name: total_amount
  type: number
- description: ''
  name: balance
  type: number
- description: ''
  name: status
  type: string
- description: ''
  name: line_items
  type: array
- description: ''
  name: remote_was_deleted
  type: boolean
provider_name: Merge
provider_slug: merge
schema_file: json-schema/accounting-api-invoice-schema.json
slug: accounting-api-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/accounting-api-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"An invoice from a connected accounting system in the Merge Unified API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_id\": { \"type\": \"string\" },\n    \"type\": { \"type\": \"string\", \"enum\": [\"ACCOUNTS_RECEIVABLE\", \"ACCOUNTS_PAYABLE\"] },\n    \"contact\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"number\": { \"type\": \"string\", \"description\": \"Invoice number.\" },\n    \"issue_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"due_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"paid_on_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"memo\": { \"type\": \"string\" },\n\
  \    \"currency\": { \"type\": \"string\", \"description\": \"ISO 4217 currency code.\" },\n    \"total_discount\": { \"type\": \"number\" },\n    \"sub_total\": { \"type\": \"number\" },\n    \"total_tax_amount\": { \"type\": \"number\" },\n    \"total_amount\": { \"type\": \"number\" },\n    \"balance\": { \"type\": \"number\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"DRAFT\", \"SUBMITTED\", \"PARTIALLY_PAID\", \"PAID\", \"OVERDUE\", \"VOIDED\"] },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n          \"description\": { \"type\": \"string\" },\n          \"unit_price\": { \"type\": \"number\" },\n          \"quantity\": { \"type\": \"number\" },\n          \"total_amount\": { \"type\": \"number\" },\n          \"account\": { \"type\": \"string\", \"format\": \"uuid\" },\n          \"item\": { \"type\": \"string\", \"format\"\
  : \"uuid\" }\n        }\n      }\n    },\n    \"remote_was_deleted\": { \"type\": \"boolean\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/accounting-api-invoice-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Invoice
---
