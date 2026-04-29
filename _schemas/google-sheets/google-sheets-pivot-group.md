---
description: A single grouping (either row or column) in a pivot table.
layout: schema
name: PivotGroup
properties_list:
- description: The column offset of the source range that this grouping is based on.
  name: sourceColumnOffset
  type: integer
- description: True if the pivot table should include the totals for this grouping.
  name: showTotals
  type: boolean
- description: The order the values in this group should be sorted.
  name: sortOrder
  type: string
- description: True if the headings in this pivot group should be repeated.
  name: repeatHeadings
  type: boolean
- description: The labels to use for the row/column groups which can be customized.
  name: label
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-group-schema.json
slug: google-sheets-pivot-group
source_filename: google-sheets-pivot-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotGroup\",\n  \"type\": \"object\",\n  \"description\": \"A single grouping (either row or column) in a pivot table.\",\n  \"properties\": {\n    \"sourceColumnOffset\": {\n      \"type\": \"integer\",\n      \"description\": \"The column offset of the source range that this grouping is based on.\"\n    },\n    \"showTotals\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the pivot table should include the totals for this grouping.\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"description\": \"The order the values in this group should be sorted.\"\n    },\n    \"repeatHeadings\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the headings in this pivot group should be repeated.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The labels to use for the row/column groups which can be customized.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-group-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotGroup
---
