---
description: Additional properties of a DATA_SOURCE sheet.
layout: schema
name: DataSourceSheetProperties
properties_list:
- description: ID of the DataSource the sheet is connected to.
  name: dataSourceId
  type: string
- description: The columns displayed on the sheet.
  name: columns
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-sheet-properties-schema.json
slug: google-sheets-data-source-sheet-properties
source_filename: google-sheets-data-source-sheet-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceSheetProperties\",\n  \"type\": \"object\",\n  \"description\": \"Additional properties of a DATA_SOURCE sheet.\",\n  \"properties\": {\n    \"dataSourceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the DataSource the sheet is connected to.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"The columns displayed on the sheet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-sheet-properties-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceSheetProperties
---
