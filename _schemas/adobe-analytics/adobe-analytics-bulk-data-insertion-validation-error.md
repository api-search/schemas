---
description: A single validation error from file validation
layout: schema
name: ValidationError
properties_list:
- description: Row number where the error occurred (1-indexed)
  name: row
  type: integer
- description: Column name where the error occurred
  name: column
  type: string
- description: Description of the validation error
  name: message
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-bulk-data-insertion-validation-error-schema.json
slug: adobe-analytics-bulk-data-insertion-validation-error
source_filename: adobe-analytics-bulk-data-insertion-validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single validation error from file validation\",\n  \"properties\": {\n    \"row\": {\n      \"type\": \"integer\",\n      \"description\": \"Row number where the error occurred (1-indexed)\",\n      \"example\": 10\n    },\n    \"column\": {\n      \"type\": \"string\",\n      \"description\": \"Column name where the error occurred\",\n      \"example\": \"example_value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the validation error\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidationError\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-bulk-data-insertion-validation-error-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ValidationError
---
