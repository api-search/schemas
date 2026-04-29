---
description: ''
layout: schema
name: PaginationResponse
properties_list:
- description: Denotes if the 'total' property is an estimation
  name: isEstimatedTotal
  type: boolean
- description: Next cursor to be sent, will be null when there are no more results
  name: next
  type: string
- description: Previous cursor, currently not supported
  name: prev
  type: integer
- description: Total number of rows in the screen
  name: total
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-universal-screening-pagination-response-schema.json
slug: factset-universal-screening-pagination-response
source_filename: factset-universal-screening-pagination-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isEstimatedTotal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Denotes if the 'total' property is an estimation\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"Next cursor to be sent, will be null when there are no more results\"\n    },\n    \"prev\": {\n      \"type\": \"integer\",\n      \"description\": \"Previous cursor, currently not supported\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the screen\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-universal-screening-pagination-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PaginationResponse
---
