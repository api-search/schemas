---
description: ''
layout: schema
name: fixedIncomeBenchmarkConstituent
properties_list:
- description: Benchmark Id
  name: fsymId
  type: string
- description: Date of weight and shares.
  name: date
  type: string
- description: FactSet Security Identifier (-S).
  name: fsymSecurityId
  type: string
- description: Weight of Security in benchmark (percent).
  name: weightClose
  type: number
- description: Amount Outstanding for the Fixed Income Security.
  name: amountOutstanding
  type: number
- description: Fixed Income Price of security held.
  name: price
  type: number
- description: Market value adjusted. Market Value represented in Millions.
  name: adjMarketValue
  type: number
- description: Identifier specified in the request
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-fixed-income-benchmark-constituent-schema.json
slug: factset-benchmarks-fixed-income-benchmark-constituent
source_filename: factset-benchmarks-fixed-income-benchmark-constituent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"fixedIncomeBenchmarkConstituent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Id\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of weight and shares.\"\n    },\n    \"fsymSecurityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier (-S).\"\n    },\n    \"weightClose\": {\n      \"type\": \"number\",\n      \"description\": \"Weight of Security in benchmark (percent).\"\n    },\n    \"amountOutstanding\": {\n      \"type\": \"number\",\n      \"description\": \"Amount Outstanding for the Fixed Income Security.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Fixed Income Price of security held.\"\n    },\n    \"adjMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Market value\
  \ adjusted. Market Value represented in Millions.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier specified in the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-fixed-income-benchmark-constituent-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: fixedIncomeBenchmarkConstituent
---
