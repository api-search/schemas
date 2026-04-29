---
description: List of pagination objects
layout: schema
name: pagination
properties_list:
- description: Total number of files the API returns for a particular query
  name: total
  type: integer
- description: Boolean value that represents whether the total count of files returned is exact or an estimate. This is defaulted to False as the API should always return the exact count
  name: isEstimatedTotal
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-pagination-schema.json
slug: factset-tick-history-pagination
source_filename: factset-tick-history-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"pagination\",\n  \"type\": \"object\",\n  \"description\": \"List of pagination objects\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of files the API returns for a particular query\"\n    },\n    \"isEstimatedTotal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value that represents whether the total count of files returned is exact or an estimate. This is defaulted to False as the API should always return the exact count\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-pagination-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: pagination
---
