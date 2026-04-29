---
description: Paginated list of budget line items.
layout: schema
name: BudgetList
properties_list:
- description: Array of budget records.
  name: data
  type: array
- description: Cursor for the next page.
  name: next_cursor
  type: string
- description: Number of records returned.
  name: count
  type: integer
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-budget-list-schema.json
slug: unified-api-budget-list
source_filename: unified-api-budget-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-budget-list-schema.json\",\n  \"title\": \"BudgetList\",\n  \"description\": \"Paginated list of budget line items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of budget records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Budget\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page.\",\n      \"example\": \"eyJpZCI6MTIzfQ==\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records returned.\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-budget-list-schema.json
tags:
- Accounting
- Construction
- Integration
title: BudgetList
---
