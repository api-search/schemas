---
description: A sort order associated with a specific column or row.
layout: schema
name: SortSpec
properties_list:
- description: The dimension the sort should be applied to.
  name: dimensionIndex
  type: integer
- description: The order data should be sorted.
  name: sortOrder
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-sort-spec-schema.json
slug: google-sheets-sort-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortSpec\",\n  \"type\": \"object\",\n  \"description\": \"A sort order associated with a specific column or row.\",\n  \"properties\": {\n    \"dimensionIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The dimension the sort should be applied to.\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"description\": \"The order data should be sorted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-sort-spec-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: SortSpec
---
