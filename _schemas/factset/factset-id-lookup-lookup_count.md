---
description: Returns the count of on entities
layout: schema
name: lookup_count
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: is_success
  type: integer
- description: Array of Lookup details for the query
  name: results
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-id-lookup-lookup_count-schema.json
slug: factset-id-lookup-lookup_count
source_filename: factset-id-lookup-lookup_count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"lookup_count\",\n  \"type\": \"object\",\n  \"description\": \"Returns the count of on entities\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\"\n    },\n    \"is_success\": {\n      \"type\": \"integer\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of Lookup details for the query\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-id-lookup-lookup_count-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: lookup_count
---
