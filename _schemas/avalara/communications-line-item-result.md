---
description: LineItemResult schema from Avalara API
layout: schema
name: LineItemResult
properties_list:
- description: Line item reference
  name: ref
  type: string
- description: ''
  name: txs
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-line-item-result-schema.json
slug: communications-line-item-result
source_filename: communications-line-item-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-line-item-result-schema.json\",\n  \"title\": \"LineItemResult\",\n  \"description\": \"LineItemResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"Line item reference\"\n    },\n    \"txs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-line-item-result-schema.json
tags:
- Taxes
title: LineItemResult
---
