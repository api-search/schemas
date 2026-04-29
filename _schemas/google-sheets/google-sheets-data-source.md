---
description: Information about an external data source in the spreadsheet.
layout: schema
name: DataSource
properties_list:
- description: The spreadsheet-scoped unique ID that identifies the data source.
  name: dataSourceId
  type: string
- description: All calculated columns in the data source.
  name: calculatedColumns
  type: array
- description: The ID of the Sheet connected with the data source.
  name: sheetId
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-schema.json
slug: google-sheets-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSource\",\n  \"type\": \"object\",\n  \"description\": \"Information about an external data source in the spreadsheet.\",\n  \"properties\": {\n    \"dataSourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The spreadsheet-scoped unique ID that identifies the data source.\"\n    },\n    \"calculatedColumns\": {\n      \"type\": \"array\",\n      \"description\": \"All calculated columns in the data source.\"\n    },\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the Sheet connected with the data source.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSource
---
