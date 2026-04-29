---
description: Paginated list of cost codes.
layout: schema
name: CostCodeList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: next_cursor
  type: string
- description: ''
  name: count
  type: integer
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-cost-code-list-schema.json
slug: unified-api-cost-code-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-cost-code-list-schema.json\",\n  \"title\": \"CostCodeList\",\n  \"description\": \"Paginated list of cost codes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CostCode\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"example\": \"eyJpZCI6MTIzfQ==\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-cost-code-list-schema.json
tags:
- Accounting
- Construction
- Integration
title: CostCodeList
---
