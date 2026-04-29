---
description: ''
layout: schema
name: batchErrorObject
properties_list:
- description: A UUID for this particular occurrence of the problem.
  name: id
  type: string
- description: status
  name: code
  type: string
- description: The Endpoint path {package}/version/{endpoint}
  name: links
  type: object
- description: The plain text error message
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-batch-error-object-schema.json
slug: factset-global-prices-batch-error-object
source_filename: factset-global-prices-batch-error-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"batchErrorObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A UUID for this particular occurrence of the problem.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"status\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"The Endpoint path {package}/version/{endpoint}\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-batch-error-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: batchErrorObject
---
