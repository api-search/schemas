---
description: error
layout: schema
name: ErrorObject
properties_list:
- description: A UUID for this particular occurrence of the problem.
  name: id
  type: string
- description: status
  name: code
  type: string
- description: The plain text error message
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-error-object-schema.json
slug: factset-tick-history-error-object
source_filename: factset-tick-history-error-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorObject\",\n  \"type\": \"object\",\n  \"description\": \"error\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A UUID for this particular occurrence of the problem.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"status\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-error-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ErrorObject
---
