---
description: Data about each cell in a row.
layout: schema
name: RowData
properties_list:
- description: The values in the row, one per column.
  name: values
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-row-data-schema.json
slug: google-sheets-row-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RowData\",\n  \"type\": \"object\",\n  \"description\": \"Data about each cell in a row.\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The values in the row, one per column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-row-data-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: RowData
---
