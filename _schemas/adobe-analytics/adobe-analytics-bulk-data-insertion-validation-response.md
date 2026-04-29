---
description: Result of a file validation request
layout: schema
name: ValidationResponse
properties_list:
- description: Whether the file passed all validation checks
  name: success
  type: boolean
- description: Summary validation message
  name: message
  type: string
- description: List of validation errors found in the file
  name: errors
  type: array
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-bulk-data-insertion-validation-response-schema.json
slug: adobe-analytics-bulk-data-insertion-validation-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Result of a file validation request\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file passed all validation checks\",\n      \"example\": true\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Summary validation message\",\n      \"example\": \"example_value\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation errors found in the file\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single validation error from file validation\",\n        \"properties\": {\n          \"row\": {\n            \"type\": \"integer\",\n            \"description\": \"Row number where the error occurred (1-indexed)\",\n            \"example\": 10\n          },\n          \"column\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Column name where the error occurred\",\n            \"example\": \"example_value\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the validation error\",\n            \"example\": \"example_value\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidationResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-bulk-data-insertion-validation-response-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ValidationResponse
---
