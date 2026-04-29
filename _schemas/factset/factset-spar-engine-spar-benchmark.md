---
description: ''
layout: schema
name: SPARBenchmark
properties_list:
- description: Benchmark identifier
  name: id
  type: string
- description: Benchmark Name
  name: name
  type: string
- description: List of SPAR identifiers
  name: identifiers
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-spar-engine-spar-benchmark-schema.json
slug: factset-spar-engine-spar-benchmark
source_filename: factset-spar-engine-spar-benchmark-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SPARBenchmark\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Name\"\n    },\n    \"identifiers\": {\n      \"type\": \"array\",\n      \"description\": \"List of SPAR identifiers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-spar-engine-spar-benchmark-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SPARBenchmark
---
