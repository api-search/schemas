---
description: ''
layout: schema
name: benchmarkRatios
properties_list:
- description: Requested Identifier. Must be a valid Benchmark Identifier recognized by FactSet.
  name: fsymId
  type: string
- description: The respective date for values as of the date requested in YYYY-MM-DD format.
  name: date
  type: string
- description: Proper Name of Index.
  name: name
  type: string
- description: Benchmark Identifier specified in the request.
  name: requestId
  type: string
- description: Metric requested
  name: metric
  type: string
- description: The periodicity submitted in the request.
  name: periodicity
  type: string
- description: The currency submitted in the request.
  name: currency
  type: string
- description: Ratio value based on the metric requested.
  name: value
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-benchmark-ratios-schema.json
slug: factset-benchmarks-benchmark-ratios
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"benchmarkRatios\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Requested Identifier. Must be a valid Benchmark Identifier recognized by FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The respective date for values as of the date requested in YYYY-MM-DD format.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Proper Name of Index.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Identifier specified in the request.\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"Metric requested\"\n    },\n    \"periodicity\": {\n      \"type\": \"string\",\n      \"description\": \"The periodicity submitted in the request.\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The currency submitted in the request.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Ratio value based on the metric requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-benchmark-ratios-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: benchmarkRatios
---
