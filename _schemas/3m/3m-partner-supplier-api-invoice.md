---
description: An invoice issued by 3M for an order
layout: schema
name: Invoice
properties_list:
- description: Unique invoice identifier
  name: invoiceId
  type: string
- description: Associated order identifier
  name: orderId
  type: string
- description: Date the invoice was issued
  name: invoiceDate
  type: string
- description: Payment due date
  name: dueDate
  type: string
- description: Total invoice amount
  name: totalAmount
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Invoice payment status
  name: status
  type: string
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-invoice-schema.json
slug: 3m-partner-supplier-api-invoice
source_filename: 3m-partner-supplier-api-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"An invoice issued by 3M for an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique invoice identifier\",\n      \"example\": \"INV-22222\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated order identifier\",\n      \"example\": \"ORD-67890\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the invoice was issued\",\n      \"example\": \"2025-03-18\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Payment due date\",\n      \"example\": \"2025-04-17\"\n    },\n\
  \    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount\",\n      \"example\": 499.95\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice payment status\",\n      \"enum\": [\n        \"unpaid\",\n        \"paid\",\n        \"overdue\",\n        \"disputed\"\n      ],\n      \"example\": \"unpaid\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-invoice-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: Invoice
---
