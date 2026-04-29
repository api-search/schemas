---
description: The response when updating a range of values in a spreadsheet by data filter.
layout: schema
name: BatchUpdateValuesByDataFilterResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: ''
  name: totalUpdatedRows
  type: integer
- description: ''
  name: totalUpdatedColumns
  type: integer
- description: ''
  name: totalUpdatedCells
  type: integer
- description: ''
  name: totalUpdatedSheets
  type: integer
- description: ''
  name: responses
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-batch-update-values-by-data-filter-response-schema.json
slug: google-sheets-batch-update-values-by-data-filter-response
source_filename: google-sheets-batch-update-values-by-data-filter-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateValuesByDataFilterResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when updating a range of values in a spreadsheet by data filter.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"totalUpdatedRows\": {\n      \"type\": \"integer\"\n    },\n    \"totalUpdatedColumns\": {\n      \"type\": \"integer\"\n    },\n    \"totalUpdatedCells\": {\n      \"type\": \"integer\"\n    },\n    \"totalUpdatedSheets\": {\n      \"type\": \"integer\"\n    },\n    \"responses\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-batch-update-values-by-data-filter-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BatchUpdateValuesByDataFilterResponse
---
