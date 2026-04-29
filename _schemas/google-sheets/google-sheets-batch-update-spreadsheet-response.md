---
description: The reply for batch updating a spreadsheet.
layout: schema
name: BatchUpdateSpreadsheetResponse
properties_list:
- description: The spreadsheet the updates were applied to.
  name: spreadsheetId
  type: string
- description: The reply of the updates.
  name: replies
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-batch-update-spreadsheet-response-schema.json
slug: google-sheets-batch-update-spreadsheet-response
source_filename: google-sheets-batch-update-spreadsheet-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateSpreadsheetResponse\",\n  \"type\": \"object\",\n  \"description\": \"The reply for batch updating a spreadsheet.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet the updates were applied to.\"\n    },\n    \"replies\": {\n      \"type\": \"array\",\n      \"description\": \"The reply of the updates.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-batch-update-spreadsheet-response-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BatchUpdateSpreadsheetResponse
---
