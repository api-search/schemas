---
description: An error in a cell.
layout: schema
name: ErrorValue
properties_list:
- description: The type of error.
  name: type
  type: string
- description: A message with more information about the error.
  name: message
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-error-value-schema.json
slug: google-sheets-error-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorValue\",\n  \"type\": \"object\",\n  \"description\": \"An error in a cell.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of error.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A message with more information about the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-error-value-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ErrorValue
---
