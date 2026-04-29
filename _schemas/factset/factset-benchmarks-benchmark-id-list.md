---
description: ''
layout: schema
name: benchmarkIdList
properties_list:
- description: Benchmark Id
  name: fsymId
  type: string
- description: Name of the Benchmark ID
  name: name
  type: string
- description: Name of the Benchmarks Family
  name: familyName
  type: string
- description: Market grouping related to the Benchmark Family
  name: market
  type: string
- description: Extended name or description of Benchmark Family & Market
  name: categoryDescription
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-benchmark-id-list-schema.json
slug: factset-benchmarks-benchmark-id-list
source_filename: factset-benchmarks-benchmark-id-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"benchmarkIdList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Id\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Benchmark ID\"\n    },\n    \"familyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Benchmarks Family\"\n    },\n    \"market\": {\n      \"type\": \"string\",\n      \"description\": \"Market grouping related to the Benchmark Family\"\n    },\n    \"categoryDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Extended name or description of Benchmark Family & Market\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-benchmark-id-list-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: benchmarkIdList
---
