---
description: InvoiceResult schema from Avalara API
layout: schema
name: InvoiceResult
properties_list:
- description: Document code
  name: doc
  type: string
- description: ''
  name: itms
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-invoice-result-schema.json
slug: communications-invoice-result
source_filename: communications-invoice-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-invoice-result-schema.json\",\n  \"title\": \"InvoiceResult\",\n  \"description\": \"InvoiceResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"doc\": {\n      \"type\": \"string\",\n      \"description\": \"Document code\"\n    },\n    \"itms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItemResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-invoice-result-schema.json
tags:
- Taxes
title: InvoiceResult
---
