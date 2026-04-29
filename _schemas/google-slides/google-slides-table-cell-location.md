---
description: A location of a single table cell within a table.
layout: schema
name: TableCellLocation
properties_list:
- description: The 0-based row index.
  name: rowIndex
  type: integer
- description: The 0-based column index.
  name: columnIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-cell-location-schema.json
slug: google-slides-table-cell-location
source_filename: google-slides-table-cell-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCellLocation\",\n  \"type\": \"object\",\n  \"description\": \"A location of a single table cell within a table.\",\n  \"properties\": {\n    \"rowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The 0-based row index.\"\n    },\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The 0-based column index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-cell-location-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TableCellLocation
---
