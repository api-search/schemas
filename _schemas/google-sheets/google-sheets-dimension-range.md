---
description: A range along a single dimension on a sheet.
layout: schema
name: DimensionRange
properties_list:
- description: The sheet this span is on.
  name: sheetId
  type: integer
- description: The start (inclusive) of the span.
  name: startIndex
  type: integer
- description: The end (exclusive) of the span.
  name: endIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-dimension-range-schema.json
slug: google-sheets-dimension-range
source_filename: google-sheets-dimension-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DimensionRange\",\n  \"type\": \"object\",\n  \"description\": \"A range along a single dimension on a sheet.\",\n  \"properties\": {\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The sheet this span is on.\"\n    },\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The start (inclusive) of the span.\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The end (exclusive) of the span.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-dimension-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DimensionRange
---
