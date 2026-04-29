---
description: Standard error response wrapper.
layout: schema
name: ErrorResponse
properties_list:
- description: An array containing error details.
  name: errors
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-error-response-schema.json
slug: factset-fundamentals-error-response
source_filename: factset-fundamentals-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response wrapper.\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"An array containing error details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-error-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ErrorResponse
---
