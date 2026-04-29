---
description: The count limit on rows or columns in the pivot group.
layout: schema
name: PivotGroupLimit
properties_list:
- description: The count limit.
  name: countLimit
  type: integer
- description: The order in which the group limit is applied to the pivot table.
  name: applyOrder
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-group-limit-schema.json
slug: google-sheets-pivot-group-limit
source_filename: google-sheets-pivot-group-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotGroupLimit\",\n  \"type\": \"object\",\n  \"description\": \"The count limit on rows or columns in the pivot group.\",\n  \"properties\": {\n    \"countLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The count limit.\"\n    },\n    \"applyOrder\": {\n      \"type\": \"integer\",\n      \"description\": \"The order in which the group limit is applied to the pivot table.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-group-limit-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotGroupLimit
---
