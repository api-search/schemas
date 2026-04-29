---
description: The response when updating a range of values in a spreadsheet.
layout: schema
name: UpdateValuesResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The range (in A1 notation) that updates were applied to.
  name: updatedRange
  type: string
- description: The number of rows where at least one cell in the row was updated.
  name: updatedRows
  type: integer
- description: The number of columns where at least one cell in the column was updated.
  name: updatedColumns
  type: integer
- description: The number of cells updated.
  name: updatedCells
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-update-values-response-schema.json
slug: google-sheets-update-values-response
source_filename: google-sheets-update-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when updating a range of values in a spreadsheet.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"updatedRange\": {\n      \"type\": \"string\",\n      \"description\": \"The range (in A1 notation) that updates were applied to.\"\n    },\n    \"updatedRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of rows where at least one cell in the row was updated.\"\n    },\n    \"updatedColumns\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of columns where at least one cell in the column was updated.\"\n    },\n    \"updatedCells\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of cells updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-update-values-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: UpdateValuesResponse
---
