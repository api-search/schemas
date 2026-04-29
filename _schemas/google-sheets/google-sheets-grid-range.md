---
description: A range on a sheet. All indexes are zero-based.
layout: schema
name: GridRange
properties_list:
- description: The sheet this range is on.
  name: sheetId
  type: integer
- description: The start row (inclusive) of the range, or not set if unbounded.
  name: startRowIndex
  type: integer
- description: The end row (exclusive) of the range, or not set if unbounded.
  name: endRowIndex
  type: integer
- description: The start column (inclusive) of the range, or not set if unbounded.
  name: startColumnIndex
  type: integer
- description: The end column (exclusive) of the range, or not set if unbounded.
  name: endColumnIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-grid-range-schema.json
slug: google-sheets-grid-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GridRange\",\n  \"type\": \"object\",\n  \"description\": \"A range on a sheet. All indexes are zero-based.\",\n  \"properties\": {\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The sheet this range is on.\"\n    },\n    \"startRowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The start row (inclusive) of the range, or not set if unbounded.\"\n    },\n    \"endRowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The end row (exclusive) of the range, or not set if unbounded.\"\n    },\n    \"startColumnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The start column (inclusive) of the range, or not set if unbounded.\"\n    },\n    \"endColumnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The end column (exclusive) of the range, or not set if unbounded.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-grid-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: GridRange
---
