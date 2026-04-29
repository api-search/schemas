---
description: The style of a table cell.
layout: schema
name: TableCellStyle
properties_list:
- description: The row span of the cell.
  name: rowSpan
  type: integer
- description: The column span of the cell.
  name: columnSpan
  type: integer
- description: The alignment of the content in the table cell.
  name: contentAlignment
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-cell-style-schema.json
slug: google-docs-v1-table-cell-style
source_filename: google-docs-v1-table-cell-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCellStyle\",\n  \"type\": \"object\",\n  \"description\": \"The style of a table cell.\",\n  \"properties\": {\n    \"rowSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The row span of the cell.\"\n    },\n    \"columnSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The column span of the cell.\"\n    },\n    \"contentAlignment\": {\n      \"type\": \"string\",\n      \"description\": \"The alignment of the content in the table cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-cell-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableCellStyle
---
