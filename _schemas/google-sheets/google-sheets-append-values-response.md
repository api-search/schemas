---
description: The response when updating a range of values by appending.
layout: schema
name: AppendValuesResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The range (in A1 notation) of the table that values are being appended to.
  name: tableRange
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-append-values-response-schema.json
slug: google-sheets-append-values-response
source_filename: google-sheets-append-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppendValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response when updating a range of values by appending.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"tableRange\": {\n      \"type\": \"string\",\n      \"description\": \"The range (in A1 notation) of the table that values are being appended to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-append-values-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: AppendValuesResponse
---
