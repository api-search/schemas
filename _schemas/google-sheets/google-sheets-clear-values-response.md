---
description: The response when clearing a range of values in a spreadsheet.
layout: schema
name: ClearValuesResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The range (in A1 notation) that was cleared.
  name: clearedRange
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-clear-values-response-schema.json
slug: google-sheets-clear-values-response
source_filename: google-sheets-clear-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClearValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when clearing a range of values in a spreadsheet.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"clearedRange\": {\n      \"type\": \"string\",\n      \"description\": \"The range (in A1 notation) that was cleared.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-clear-values-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ClearValuesResponse
---
