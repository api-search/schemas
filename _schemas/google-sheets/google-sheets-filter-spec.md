---
description: The filter criteria associated with a specific column.
layout: schema
name: FilterSpec
properties_list:
- description: The zero-based column index.
  name: columnIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-filter-spec-schema.json
slug: google-sheets-filter-spec
source_filename: google-sheets-filter-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterSpec\",\n  \"type\": \"object\",\n  \"description\": \"The filter criteria associated with a specific column.\",\n  \"properties\": {\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based column index.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-filter-spec-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: FilterSpec
---
