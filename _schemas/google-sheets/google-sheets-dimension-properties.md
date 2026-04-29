---
description: Properties about a dimension.
layout: schema
name: DimensionProperties
properties_list:
- description: True if this dimension is being filtered.
  name: hiddenByFilter
  type: boolean
- description: True if this dimension is explicitly hidden.
  name: hiddenByUser
  type: boolean
- description: The height (for rows) or width (for columns) of the dimension in pixels.
  name: pixelSize
  type: integer
- description: The developer metadata associated with a single row or column.
  name: developerMetadata
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-dimension-properties-schema.json
slug: google-sheets-dimension-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DimensionProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties about a dimension.\",\n  \"properties\": {\n    \"hiddenByFilter\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this dimension is being filtered.\"\n    },\n    \"hiddenByUser\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this dimension is explicitly hidden.\"\n    },\n    \"pixelSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The height (for rows) or width (for columns) of the dimension in pixels.\"\n    },\n    \"developerMetadata\": {\n      \"type\": \"array\",\n      \"description\": \"The developer metadata associated with a single row or column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-dimension-properties-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DimensionProperties
---
