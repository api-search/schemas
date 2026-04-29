---
description: A rule describing a conditional format.
layout: schema
name: ConditionalFormatRule
properties_list:
- description: The ranges that are formatted if the condition is true.
  name: ranges
  type: array
- description: The formatting is either on or off according to the rule.
  name: booleanRule
  type: object
- description: The formatting will vary based on the gradients in the rule.
  name: gradientRule
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-conditional-format-rule-schema.json
slug: google-sheets-conditional-format-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConditionalFormatRule\",\n  \"type\": \"object\",\n  \"description\": \"A rule describing a conditional format.\",\n  \"properties\": {\n    \"ranges\": {\n      \"type\": \"array\",\n      \"description\": \"The ranges that are formatted if the condition is true.\"\n    },\n    \"booleanRule\": {\n      \"type\": \"object\",\n      \"description\": \"The formatting is either on or off according to the rule.\"\n    },\n    \"gradientRule\": {\n      \"type\": \"object\",\n      \"description\": \"The formatting will vary based on the gradients in the rule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-conditional-format-rule-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ConditionalFormatRule
---
