---
description: Invoice schema from Avalara API
layout: schema
name: Invoice
properties_list:
- description: Document code
  name: doc
  type: string
- description: Commit indicator
  name: cmmt
  type: boolean
- description: ''
  name: bill
  type: object
- description: Customer type
  name: cust
  type: integer
- description: Invoice date
  name: date
  type: string
- description: Line items on the invoice
  name: itms
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-invoice-schema.json
slug: communications-invoice
source_filename: communications-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"Invoice schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"doc\": {\n      \"type\": \"string\",\n      \"description\": \"Document code\"\n    },\n    \"cmmt\": {\n      \"type\": \"boolean\",\n      \"description\": \"Commit indicator\"\n    },\n    \"bill\": {\n      \"$ref\": \"#/components/schemas/Location\"\n    },\n    \"cust\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer type\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Invoice date\"\n    },\n    \"itms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"description\": \"Line\
  \ items on the invoice\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-invoice-schema.json
tags:
- Taxes
title: Invoice
---
