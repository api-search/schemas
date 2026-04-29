---
description: The contents and style of a row in a table.
layout: schema
name: TableRow
properties_list:
- description: The zero-based start index of this row.
  name: startIndex
  type: integer
- description: The zero-based end index of this row, exclusive.
  name: endIndex
  type: integer
- description: The contents and style of each cell in this row.
  name: tableCells
  type: array
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
- description: ''
  name: suggestedTableRowStyleChanges
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-row-schema.json
slug: google-docs-v1-table-row
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableRow\",\n  \"type\": \"object\",\n  \"description\": \"The contents and style of a row in a table.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based start index of this row.\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based end index of this row, exclusive.\"\n    },\n    \"tableCells\": {\n      \"type\": \"array\",\n      \"description\": \"The contents and style of each cell in this row.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTableRowStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-row-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableRow
---
