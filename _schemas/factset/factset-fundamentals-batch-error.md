---
description: Error information for a failed batch request.
layout: schema
name: BatchError
properties_list:
- description: A UUID for this particular occurrence of the problem.
  name: id
  type: string
- description: Error code.
  name: code
  type: string
- description: The plain text error message.
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-batch-error-schema.json
slug: factset-fundamentals-batch-error
source_filename: factset-fundamentals-batch-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchError\",\n  \"type\": \"['object', 'null']\",\n  \"description\": \"Error information for a failed batch request.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A UUID for this particular occurrence of the problem.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-batch-error-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: BatchError
---
