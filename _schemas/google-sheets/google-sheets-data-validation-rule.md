---
description: A data validation rule.
layout: schema
name: DataValidationRule
properties_list:
- description: A message to show the user when adding data to the cell.
  name: inputMessage
  type: string
- description: True if invalid data should be rejected.
  name: strict
  type: boolean
- description: True if the UI should be customized based on the kind of condition.
  name: showCustomUi
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-validation-rule-schema.json
slug: google-sheets-data-validation-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataValidationRule\",\n  \"type\": \"object\",\n  \"description\": \"A data validation rule.\",\n  \"properties\": {\n    \"inputMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A message to show the user when adding data to the cell.\"\n    },\n    \"strict\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if invalid data should be rejected.\"\n    },\n    \"showCustomUi\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the UI should be customized based on the kind of condition.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-validation-rule-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataValidationRule
---
