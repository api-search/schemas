---
description: A sales invoice in Sage Accounting representing a customer billing record.
layout: schema
name: Sage Sales Invoice
properties_list:
- description: Unique invoice identifier
  name: id
  type: string
- description: Invoice reference number display
  name: displayed_as
  type: string
- description: Invoice date
  name: date
  type: string
- description: Payment due date
  name: due_date
  type: string
- description: Invoice reference number
  name: reference
  type: string
- description: Current invoice status
  name: status
  type: object
- description: Customer contact reference
  name: contact
  type: object
- description: Invoice line items
  name: line_items
  type: array
- description: Total pre-tax amount
  name: net_amount
  type: number
- description: Total tax amount
  name: tax_amount
  type: number
- description: Total invoice amount including tax
  name: total_amount
  type: number
- description: Remaining unpaid amount
  name: outstanding_amount
  type: number
- description: ''
  name: currency
  type: object
provider_name: Sage
provider_slug: sage
schema_file: json-schema/sage-invoice-schema.json
slug: sage-invoice
source_filename: sage-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sage/main/json-schema/sage-invoice-schema.json\",\n  \"title\": \"Sage Sales Invoice\",\n  \"description\": \"A sales invoice in Sage Accounting representing a customer billing record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique invoice identifier\"\n    },\n    \"displayed_as\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice reference number display\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Invoice date\"\n    },\n    \"due_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Payment due date\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice reference number\"\n    },\n    \"status\": {\n     \
  \ \"type\": \"object\",\n      \"description\": \"Current invoice status\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"enum\": [\"DRAFT\", \"SENT\", \"PAID\", \"VOID\"]\n        },\n        \"displayed_as\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"contact\": {\n      \"type\": \"object\",\n      \"description\": \"Customer contact reference\",\n      \"properties\": {\n        \"id\": {\"type\": \"string\"},\n        \"displayed_as\": {\"type\": \"string\"}\n      }\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"description\": \"Invoice line items\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\"type\": \"string\"},\n          \"description\": {\"type\": \"string\"},\n          \"quantity\": {\"type\": \"number\"},\n          \"unit_price\": {\"type\": \"number\"},\n          \"net_amount\": {\"type\": \"number\"},\n          \"tax_amount\"\
  : {\"type\": \"number\"},\n          \"total_amount\": {\"type\": \"number\"},\n          \"ledger_account\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\"type\": \"string\"},\n              \"displayed_as\": {\"type\": \"string\"}\n            }\n          },\n          \"tax_rate\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\"type\": \"string\"},\n              \"displayed_as\": {\"type\": \"string\"}\n            }\n          }\n        }\n      }\n    },\n    \"net_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total pre-tax amount\"\n    },\n    \"tax_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax amount\"\n    },\n    \"total_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount including tax\"\n    },\n    \"outstanding_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Remaining unpaid\
  \ amount\"\n    },\n    \"currency\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\"type\": \"string\"},\n        \"displayed_as\": {\"type\": \"string\"}\n      }\n    }\n  },\n  \"required\": [\"id\", \"date\", \"contact\", \"line_items\", \"total_amount\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/json-schema/sage-invoice-schema.json
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
title: Sage Sales Invoice
---
