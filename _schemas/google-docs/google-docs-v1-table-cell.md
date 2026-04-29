---
description: The contents and style of a cell in a table.
layout: schema
name: TableCell
properties_list:
- description: ''
  name: startIndex
  type: integer
- description: ''
  name: endIndex
  type: integer
- description: The content of the cell.
  name: content
  type: array
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
- description: ''
  name: suggestedTableCellStyleChanges
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-cell-schema.json
slug: google-docs-v1-table-cell
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCell\",\n  \"type\": \"object\",\n  \"description\": \"The contents and style of a cell in a table.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The content of the cell.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTableCellStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-cell-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableCell
---
