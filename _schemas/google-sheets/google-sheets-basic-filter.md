---
description: The default filter associated with a sheet.
layout: schema
name: BasicFilter
properties_list:
- description: The sort order per column.
  name: sortSpecs
  type: array
- description: The criteria for showing/hiding values per column.
  name: criteria
  type: object
- description: The filter criteria per column.
  name: filterSpecs
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-basic-filter-schema.json
slug: google-sheets-basic-filter
source_filename: google-sheets-basic-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BasicFilter\",\n  \"type\": \"object\",\n  \"description\": \"The default filter associated with a sheet.\",\n  \"properties\": {\n    \"sortSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"The sort order per column.\"\n    },\n    \"criteria\": {\n      \"type\": \"object\",\n      \"description\": \"The criteria for showing/hiding values per column.\"\n    },\n    \"filterSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"The filter criteria per column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-basic-filter-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BasicFilter
---
