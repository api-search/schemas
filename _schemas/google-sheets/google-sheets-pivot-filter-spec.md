---
description: The pivot table filter criteria associated with a specific source column offset.
layout: schema
name: PivotFilterSpec
properties_list:
- description: The zero-based column offset of the source range.
  name: columnOffsetIndex
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-filter-spec-schema.json
slug: google-sheets-pivot-filter-spec
source_filename: google-sheets-pivot-filter-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotFilterSpec\",\n  \"type\": \"object\",\n  \"description\": \"The pivot table filter criteria associated with a specific source column offset.\",\n  \"properties\": {\n    \"columnOffsetIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based column offset of the source range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-filter-spec-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotFilterSpec
---
