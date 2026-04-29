---
description: The kinds of value that a cell in a spreadsheet can have.
layout: schema
name: ExtendedValue
properties_list:
- description: Represents a double value.
  name: numberValue
  type: number
- description: Represents a string value.
  name: stringValue
  type: string
- description: Represents a boolean value.
  name: boolValue
  type: boolean
- description: Represents a formula.
  name: formulaValue
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-extended-value-schema.json
slug: google-sheets-extended-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtendedValue\",\n  \"type\": \"object\",\n  \"description\": \"The kinds of value that a cell in a spreadsheet can have.\",\n  \"properties\": {\n    \"numberValue\": {\n      \"type\": \"number\",\n      \"description\": \"Represents a double value.\"\n    },\n    \"stringValue\": {\n      \"type\": \"string\",\n      \"description\": \"Represents a string value.\"\n    },\n    \"boolValue\": {\n      \"type\": \"boolean\",\n      \"description\": \"Represents a boolean value.\"\n    },\n    \"formulaValue\": {\n      \"type\": \"string\",\n      \"description\": \"Represents a formula.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-extended-value-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ExtendedValue
---
