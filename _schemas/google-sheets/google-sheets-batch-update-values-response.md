---
description: The response when updating a range of values in a spreadsheet.
layout: schema
name: BatchUpdateValuesResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The total number of rows where at least one cell in the row was updated.
  name: totalUpdatedRows
  type: integer
- description: The total number of columns where at least one cell in the column was updated.
  name: totalUpdatedColumns
  type: integer
- description: The total number of cells updated.
  name: totalUpdatedCells
  type: integer
- description: The total number of sheets where at least one cell in the sheet was updated.
  name: totalUpdatedSheets
  type: integer
- description: One UpdateValuesResponse per requested range, in the same order as the requests appeared.
  name: responses
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-batch-update-values-response-schema.json
slug: google-sheets-batch-update-values-response
source_filename: google-sheets-batch-update-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when updating a range of values in a spreadsheet.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"totalUpdatedRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of rows where at least one cell in the row was updated.\"\n    },\n    \"totalUpdatedColumns\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of columns where at least one cell in the column was updated.\"\n    },\n    \"totalUpdatedCells\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of cells updated.\"\n    },\n    \"totalUpdatedSheets\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of sheets where at least\
  \ one cell in the sheet was updated.\"\n    },\n    \"responses\": {\n      \"type\": \"array\",\n      \"description\": \"One UpdateValuesResponse per requested range, in the same order as the requests appeared.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-batch-update-values-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BatchUpdateValuesResponse
---
