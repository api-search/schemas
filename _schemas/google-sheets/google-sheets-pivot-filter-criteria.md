---
description: Criteria for showing/hiding rows in a pivot table.
layout: schema
name: PivotFilterCriteria
properties_list:
- description: Values that should be included.
  name: visibleValues
  type: array
- description: Whether values are visible by default.
  name: visibleByDefault
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-pivot-filter-criteria-schema.json
slug: google-sheets-pivot-filter-criteria
source_filename: google-sheets-pivot-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PivotFilterCriteria\",\n  \"type\": \"object\",\n  \"description\": \"Criteria for showing/hiding rows in a pivot table.\",\n  \"properties\": {\n    \"visibleValues\": {\n      \"type\": \"array\",\n      \"description\": \"Values that should be included.\"\n    },\n    \"visibleByDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether values are visible by default.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-pivot-filter-criteria-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: PivotFilterCriteria
---
