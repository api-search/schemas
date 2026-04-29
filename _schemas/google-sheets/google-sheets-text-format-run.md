---
description: A run of a text format.
layout: schema
name: TextFormatRun
properties_list:
- description: The character index where this run starts (zero-based).
  name: startIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-text-format-run-schema.json
slug: google-sheets-text-format-run
source_filename: google-sheets-text-format-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextFormatRun\",\n  \"type\": \"object\",\n  \"description\": \"A run of a text format.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The character index where this run starts (zero-based).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-text-format-run-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: TextFormatRun
---
