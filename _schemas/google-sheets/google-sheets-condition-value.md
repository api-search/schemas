---
description: The value of the condition.
layout: schema
name: ConditionValue
properties_list:
- description: A relative date.
  name: relativeDate
  type: string
- description: A value the condition is based on.
  name: userEnteredValue
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-condition-value-schema.json
slug: google-sheets-condition-value
source_filename: google-sheets-condition-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConditionValue\",\n  \"type\": \"object\",\n  \"description\": \"The value of the condition.\",\n  \"properties\": {\n    \"relativeDate\": {\n      \"type\": \"string\",\n      \"description\": \"A relative date.\"\n    },\n    \"userEnteredValue\": {\n      \"type\": \"string\",\n      \"description\": \"A value the condition is based on.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-condition-value-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ConditionValue
---
