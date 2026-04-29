---
description: ''
layout: schema
name: errorResponse
properties_list:
- description: status
  name: status
  type: string
- description: timestamp in YYYY-MM-DD HH:MM:SS.SSS
  name: timestamp
  type: string
- description: The Endpoint path {package}/version/{endpoint}
  name: path
  type: string
- description: The plain text error message
  name: message
  type: string
- description: subErrors related to the error message. Null if not applicable.
  name: subErrors
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-error-response-schema.json
slug: factset-benchmarks-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"errorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"status\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"timestamp in YYYY-MM-DD HH:MM:SS.SSS\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The Endpoint path {package}/version/{endpoint}\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message\"\n    },\n    \"subErrors\": {\n      \"type\": \"object\",\n      \"description\": \"subErrors related to the error message. Null if not applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-error-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: errorResponse
---
