---
description: The response when clearing a range of values in a spreadsheet.
layout: schema
name: BatchClearValuesResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The ranges that were cleared, in A1 notation.
  name: clearedRanges
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-batch-clear-values-response-schema.json
slug: google-sheets-batch-clear-values-response
source_filename: google-sheets-batch-clear-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchClearValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when clearing a range of values in a spreadsheet.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"clearedRanges\": {\n      \"type\": \"array\",\n      \"description\": \"The ranges that were cleared, in A1 notation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-batch-clear-values-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BatchClearValuesResponse
---
