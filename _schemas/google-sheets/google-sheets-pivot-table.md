---
description: A pivot table.
layout: schema
name: PivotTable
properties_list:
- description: Each row grouping in the pivot table.
  name: rows
  type: array
- description: Each column grouping in the pivot table.
  name: columns
  type: array
- description: A list of values to include in the pivot table.
  name: values
  type: array
- description: An optional mapping of filters per source column offset.
  name: criteria
  type: object
- description: The filters applied to the source columns before aggregating data.
  name: filterSpecs
  type: array
- description: Whether values should be listed horizontally or vertically.
  name: valueLayout
  type: string
- description: The ID of the data source the pivot table is reading data from.
  name: dataSourceId
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-table-schema.json
slug: google-sheets-pivot-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotTable\",\n  \"type\": \"object\",\n  \"description\": \"A pivot table.\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Each row grouping in the pivot table.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"Each column grouping in the pivot table.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"A list of values to include in the pivot table.\"\n    },\n    \"criteria\": {\n      \"type\": \"object\",\n      \"description\": \"An optional mapping of filters per source column offset.\"\n    },\n    \"filterSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"The filters applied to the source columns before aggregating data.\"\n    },\n    \"valueLayout\": {\n      \"type\": \"string\",\n      \"description\": \"Whether values should be listed horizontally or vertically.\"\
  \n    },\n    \"dataSourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the data source the pivot table is reading data from.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-table-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotTable
---
