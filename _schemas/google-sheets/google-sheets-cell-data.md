---
description: Data about a specific cell.
layout: schema
name: CellData
properties_list:
- description: The formatted value of the cell. This is the value as it is shown to the user.
  name: formattedValue
  type: string
- description: A hyperlink this cell points to, if any.
  name: hyperlink
  type: string
- description: Any note on the cell.
  name: note
  type: string
- description: Runs of rich text applied to subsections of the cell.
  name: textFormatRuns
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-cell-data-schema.json
slug: google-sheets-cell-data
source_filename: google-sheets-cell-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CellData\",\n  \"type\": \"object\",\n  \"description\": \"Data about a specific cell.\",\n  \"properties\": {\n    \"formattedValue\": {\n      \"type\": \"string\",\n      \"description\": \"The formatted value of the cell. This is the value as it is shown to the user.\"\n    },\n    \"hyperlink\": {\n      \"type\": \"string\",\n      \"description\": \"A hyperlink this cell points to, if any.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"Any note on the cell.\"\n    },\n    \"textFormatRuns\": {\n      \"type\": \"array\",\n      \"description\": \"Runs of rich text applied to subsections of the cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-cell-data-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: CellData
---
