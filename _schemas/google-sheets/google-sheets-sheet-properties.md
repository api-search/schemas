---
description: Properties of a sheet.
layout: schema
name: SheetProperties
properties_list:
- description: The ID of the sheet. Must be non-negative. This field cannot be changed once set.
  name: sheetId
  type: integer
- description: The name of the sheet.
  name: title
  type: string
- description: The index of the sheet within the spreadsheet.
  name: index
  type: integer
- description: The type of sheet.
  name: sheetType
  type: string
- description: True if the sheet is hidden in the UI, false if visible.
  name: hidden
  type: boolean
- description: True if the sheet is an RTL sheet instead of an LTR sheet.
  name: rightToLeft
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-sheet-properties-schema.json
slug: google-sheets-sheet-properties
source_filename: google-sheets-sheet-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SheetProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a sheet.\",\n  \"properties\": {\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the sheet. Must be non-negative. This field cannot be changed once set.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the sheet.\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the sheet within the spreadsheet.\"\n    },\n    \"sheetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of sheet.\"\n    },\n    \"hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the sheet is hidden in the UI, false if visible.\"\n    },\n    \"rightToLeft\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the sheet is an RTL sheet instead of an LTR sheet.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-sheet-properties-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: SheetProperties
---
