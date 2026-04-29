---
description: Criteria for showing/hiding rows in a filter or filter view.
layout: schema
name: FilterCriteria
properties_list:
- description: Values that should be hidden.
  name: hiddenValues
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-filter-criteria-schema.json
slug: google-sheets-filter-criteria
source_filename: google-sheets-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterCriteria\",\n  \"type\": \"object\",\n  \"description\": \"Criteria for showing/hiding rows in a filter or filter view.\",\n  \"properties\": {\n    \"hiddenValues\": {\n      \"type\": \"array\",\n      \"description\": \"Values that should be hidden.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-filter-criteria-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: FilterCriteria
---
