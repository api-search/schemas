---
description: Location of a single cell within a table.
layout: schema
name: TableCellLocation
properties_list:
- description: The zero-based row index.
  name: rowIndex
  type: integer
- description: The zero-based column index.
  name: columnIndex
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-cell-location-schema.json
slug: google-docs-v1-table-cell-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCellLocation\",\n  \"type\": \"object\",\n  \"description\": \"Location of a single cell within a table.\",\n  \"properties\": {\n    \"rowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based row index.\"\n    },\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based column index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-cell-location-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableCellLocation
---
