---
description: A coordinate in a sheet.
layout: schema
name: GridCoordinate
properties_list:
- description: The sheet this coordinate is on.
  name: sheetId
  type: integer
- description: The row index of the coordinate.
  name: rowIndex
  type: integer
- description: The column index of the coordinate.
  name: columnIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-grid-coordinate-schema.json
slug: google-sheets-grid-coordinate
source_filename: google-sheets-grid-coordinate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GridCoordinate\",\n  \"type\": \"object\",\n  \"description\": \"A coordinate in a sheet.\",\n  \"properties\": {\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The sheet this coordinate is on.\"\n    },\n    \"rowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The row index of the coordinate.\"\n    },\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The column index of the coordinate.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-grid-coordinate-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: GridCoordinate
---
