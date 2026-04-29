---
description: A condition that can evaluate to true or false.
layout: schema
name: BooleanCondition
properties_list:
- description: The type of condition.
  name: type
  type: string
- description: The values of the condition. The number of supported values depends on the condition type.
  name: values
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-boolean-condition-schema.json
slug: google-sheets-boolean-condition
source_filename: google-sheets-boolean-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BooleanCondition\",\n  \"type\": \"object\",\n  \"description\": \"A condition that can evaluate to true or false.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of condition.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The values of the condition. The number of supported values depends on the condition type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-boolean-condition-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BooleanCondition
---
