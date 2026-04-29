---
description: ''
layout: schema
name: PaginationInfo
properties_list:
- description: ''
  name: pageNumber
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: totalPages
  type: integer
- description: ''
  name: totalCalculations
  type: integer
- description: ''
  name: nextPage
  type: string
- description: ''
  name: previousPage
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-pagination-info-schema.json
slug: factset-vault-pagination-info
source_filename: factset-vault-pagination-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageNumber\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    },\n    \"totalCalculations\": {\n      \"type\": \"integer\"\n    },\n    \"nextPage\": {\n      \"type\": \"string\"\n    },\n    \"previousPage\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-pagination-info-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PaginationInfo
---
