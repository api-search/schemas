---
description: Filter that describes what data should be selected or returned from a request.
layout: schema
name: DataFilter
properties_list:
- description: Selects data that matches the specified A1 range.
  name: a1Range
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-filter-schema.json
slug: google-sheets-data-filter
source_filename: google-sheets-data-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataFilter\",\n  \"type\": \"object\",\n  \"description\": \"Filter that describes what data should be selected or returned from a request.\",\n  \"properties\": {\n    \"a1Range\": {\n      \"type\": \"string\",\n      \"description\": \"Selects data that matches the specified A1 range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-filter-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataFilter
---
