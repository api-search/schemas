---
description: ''
layout: schema
name: errorResponse
properties_list:
- description: A short description of the error.
  name: message
  type: string
- description: Optional list of errors. e.g. Validation errors for multiple parameters
  name: errors
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-error-response-schema.json
slug: factset-signals-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"errorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the error.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Optional list of errors. e.g. Validation errors for multiple parameters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-error-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: errorResponse
---
