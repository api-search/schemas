---
description: Information about which values in a pivot group should be used for sorting.
layout: schema
name: PivotGroupSortValueBucket
properties_list:
- description: The offset in the PivotTable.values list which the values in this grouping should be sorted by.
  name: valuesIndex
  type: integer
- description: Determines the bucket from which values are chosen to sort.
  name: buckets
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-group-sort-value-bucket-schema.json
slug: google-sheets-pivot-group-sort-value-bucket
source_filename: google-sheets-pivot-group-sort-value-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotGroupSortValueBucket\",\n  \"type\": \"object\",\n  \"description\": \"Information about which values in a pivot group should be used for sorting.\",\n  \"properties\": {\n    \"valuesIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The offset in the PivotTable.values list which the values in this grouping should be sorted by.\"\n    },\n    \"buckets\": {\n      \"type\": \"array\",\n      \"description\": \"Determines the bucket from which values are chosen to sort.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-group-sort-value-bucket-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotGroupSortValueBucket
---
