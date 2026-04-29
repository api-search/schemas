---
description: ''
layout: schema
name: benchmarkConstituent
properties_list:
- description: Benchmark Id
  name: fsymId
  type: string
- description: Date of weight and shares.
  name: date
  type: string
- description: FactSet Security Identifier (-S). If Cash or Generic Id holding, response will just pass through generic id (e.g. CASH_USD).
  name: fsymSecurityId
  type: string
- description: FactSet Regional Identifier (-R). If Cash or Generic Id holding, response will just pass through generic id (e.g. CASH_USD).
  name: fsymRegionalId
  type: string
- description: Currency code for prices.
  name: currency
  type: string
- description: Weight of Security in benchmark (percent).
  name: weightClose
  type: number
- description: Shares held adjusted. Units in Millions.
  name: adjHolding
  type: number
- description: Shares held unadjusted. Units in Millions.
  name: unadjHolding
  type: number
- description: Price of shares held.
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
schema_file: json-schema/factset-benchmarks-benchmark-constituent-schema.json
slug: factset-benchmarks-benchmark-constituent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"benchmarkConstituent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Id\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of weight and shares.\"\n    },\n    \"fsymSecurityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier (-S). If Cash or Generic Id holding, response will just pass through generic id (e.g. CASH_USD).\"\n    },\n    \"fsymRegionalId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Regional Identifier (-R). If Cash or Generic Id holding, response will just pass through generic id (e.g. CASH_USD).\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for prices.\"\n    },\n    \"weightClose\": {\n      \"type\": \"number\",\n      \"description\": \"Weight\
  \ of Security in benchmark (percent).\"\n    },\n    \"adjHolding\": {\n      \"type\": \"number\",\n      \"description\": \"Shares held adjusted. Units in Millions.\"\n    },\n    \"unadjHolding\": {\n      \"type\": \"number\",\n      \"description\": \"Shares held unadjusted. Units in Millions.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Price of shares held.\"\n    },\n    \"adjMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Market value adjusted. Market Value represented in Millions.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier specified in the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-benchmark-constituent-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: benchmarkConstituent
---
