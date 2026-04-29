---
description: A Google Sheets spreadsheet resource.
layout: schema
name: Spreadsheet
properties_list:
- description: The ID of the spreadsheet. Read-only.
  name: spreadsheetId
  type: string
- description: The sheets that are part of a spreadsheet.
  name: sheets
  type: array
- description: The named ranges defined in a spreadsheet.
  name: namedRanges
  type: array
- description: The URL of the spreadsheet. Read-only.
  name: spreadsheetUrl
  type: string
- description: The developer metadata associated with a spreadsheet.
  name: developerMetadata
  type: array
- description: A list of external data sources connected to the spreadsheet.
  name: dataSources
  type: array
- description: Output only. A list of data source refresh schedules.
  name: dataSourceSchedules
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-spreadsheet-schema.json
slug: google-sheets-spreadsheet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Spreadsheet\",\n  \"type\": \"object\",\n  \"description\": \"A Google Sheets spreadsheet resource.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the spreadsheet. Read-only.\"\n    },\n    \"sheets\": {\n      \"type\": \"array\",\n      \"description\": \"The sheets that are part of a spreadsheet.\"\n    },\n    \"namedRanges\": {\n      \"type\": \"array\",\n      \"description\": \"The named ranges defined in a spreadsheet.\"\n    },\n    \"spreadsheetUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the spreadsheet. Read-only.\"\n    },\n    \"developerMetadata\": {\n      \"type\": \"array\",\n      \"description\": \"The developer metadata associated with a spreadsheet.\"\n    },\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"description\": \"A list of external data sources connected\
  \ to the spreadsheet.\"\n    },\n    \"dataSourceSchedules\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. A list of data source refresh schedules.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-spreadsheet-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Spreadsheet
---
