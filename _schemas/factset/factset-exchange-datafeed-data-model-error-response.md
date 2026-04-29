---
description: ''
layout: schema
name: errorResponse
properties_list:
- description: status
  name: status
  type: integer
- description: The plain text error message
  name: error
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-exchange-datafeed-data-model-error-response-schema.json
slug: factset-exchange-datafeed-data-model-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"errorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"status\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-exchange-datafeed-data-model-error-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: errorResponse
---
