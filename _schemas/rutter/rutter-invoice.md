---
description: An invoice from a connected accounting platform via the Rutter Unified API
layout: schema
name: Rutter Invoice
properties_list:
- description: Unique identifier for the invoice
  name: id
  type: string
- description: The ID of the customer this invoice belongs to
  name: customer_id
  type: string
- description: Current invoice status
  name: status
  type: string
- description: Total amount due on the invoice
  name: amount_due
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Date the invoice is due
  name: due_date
  type: string
- description: Line items on the invoice
  name: line_items
  type: array
provider_name: Rutter
provider_slug: rutter
schema_file: json-schema/rutter-invoice-schema.json
slug: rutter-invoice
source_filename: rutter-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rutter/json-schema/rutter-invoice-schema.json\",\n  \"title\": \"Rutter Invoice\",\n  \"description\": \"An invoice from a connected accounting platform via the Rutter Unified API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the invoice\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the customer this invoice belongs to\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"open\", \"paid\", \"voided\"],\n      \"description\": \"Current invoice status\"\n    },\n    \"amount_due\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total amount due on the invoice\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217\
  \ currency code\",\n      \"examples\": [\"USD\", \"EUR\", \"GBP\"]\n    },\n    \"due_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the invoice is due\"\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      },\n      \"description\": \"Line items on the invoice\"\n    }\n  },\n  \"required\": [\"id\", \"status\"],\n  \"$defs\": {\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"quantity\": {\n          \"type\": \"number\"\n        },\n        \"unit_price\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        },\n        \"total_amount\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rutter/refs/heads/main/json-schema/rutter-invoice-schema.json
tags:
- Accounting
- B2B
- Commerce
- Financial Data
- Payments
- Unified API
title: Rutter Invoice
---
