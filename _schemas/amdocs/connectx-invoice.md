---
description: Invoice schema from Amdocs API
layout: schema
name: Invoice
properties_list:
- description: ''
  name: invoiceId
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: customerId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: taxAmount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: lineItems
  type: array
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-invoice-schema.json
slug: connectx-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"Invoice schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"string\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"customerId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Open\",\n        \"Paid\",\n        \"Overdue\",\n        \"Cancelled\"\n      ]\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\"\n    },\n    \"taxAmount\": {\n      \"type\": \"number\"\n    },\n    \"currency\": {\n\
  \      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvoiceLineItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-invoice-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Invoice
---
