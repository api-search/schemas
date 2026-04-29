---
description: A filter view.
layout: schema
name: FilterView
properties_list:
- description: The ID of the filter view.
  name: filterViewId
  type: integer
- description: The name of the filter view.
  name: title
  type: string
- description: The named range this filter view is backed by, if any.
  name: namedRangeId
  type: string
- description: The sort order per column.
  name: sortSpecs
  type: array
- description: The criteria for showing/hiding values per column.
  name: criteria
  type: object
- description: The filter criteria for showing/hiding values per column.
  name: filterSpecs
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-filter-view-schema.json
slug: google-sheets-filter-view
source_filename: google-sheets-filter-view-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterView\",\n  \"type\": \"object\",\n  \"description\": \"A filter view.\",\n  \"properties\": {\n    \"filterViewId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the filter view.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the filter view.\"\n    },\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The named range this filter view is backed by, if any.\"\n    },\n    \"sortSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"The sort order per column.\"\n    },\n    \"criteria\": {\n      \"type\": \"object\",\n      \"description\": \"The criteria for showing/hiding values per column.\"\n    },\n    \"filterSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"The filter criteria for showing/hiding values per column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-filter-view-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: FilterView
---
