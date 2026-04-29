---
description: Properties of a grid.
layout: schema
name: GridProperties
properties_list:
- description: The number of rows in the grid.
  name: rowCount
  type: integer
- description: The number of columns in the grid.
  name: columnCount
  type: integer
- description: The number of rows that are frozen in the grid.
  name: frozenRowCount
  type: integer
- description: The number of columns that are frozen in the grid.
  name: frozenColumnCount
  type: integer
- description: True if the grid is not showing gridlines in the UI.
  name: hideGridlines
  type: boolean
- description: True if the row grouping control toggle is shown after the group.
  name: rowGroupControlAfter
  type: boolean
- description: True if the column grouping control toggle is shown after the group.
  name: columnGroupControlAfter
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-grid-properties-schema.json
slug: google-sheets-grid-properties
source_filename: google-sheets-grid-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GridProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a grid.\",\n  \"properties\": {\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of rows in the grid.\"\n    },\n    \"columnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of columns in the grid.\"\n    },\n    \"frozenRowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of rows that are frozen in the grid.\"\n    },\n    \"frozenColumnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of columns that are frozen in the grid.\"\n    },\n    \"hideGridlines\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the grid is not showing gridlines in the UI.\"\n    },\n    \"rowGroupControlAfter\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the row grouping control\
  \ toggle is shown after the group.\"\n    },\n    \"columnGroupControlAfter\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the column grouping control toggle is shown after the group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-grid-properties-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: GridProperties
---
