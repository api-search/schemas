---
description: The number format of a cell.
layout: schema
name: NumberFormat
properties_list:
- description: The type of the number format.
  name: type
  type: string
- description: Pattern string used for formatting.
  name: pattern
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-number-format-schema.json
slug: google-sheets-number-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NumberFormat\",\n  \"type\": \"object\",\n  \"description\": \"The number format of a cell.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the number format.\"\n    },\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"Pattern string used for formatting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-number-format-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: NumberFormat
---
