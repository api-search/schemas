---
description: ''
layout: schema
name: PACalculationDataSources
properties_list:
- description: List of portfilio pricing source for the PA calculation
  name: portfoliopricingsources
  type: array
- description: List of benchmark pricing source for the PA calculation
  name: benchmarkpricingsources
  type: array
- description: Use portfolio pricing sources for benchmark
  name: useportfoliopricingsourcesforbenchmark
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-pa-calculation-data-sources-schema.json
slug: factset-pa-engine-pa-calculation-data-sources
source_filename: factset-pa-engine-pa-calculation-data-sources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PACalculationDataSources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfoliopricingsources\": {\n      \"type\": \"array\",\n      \"description\": \"List of portfilio pricing source for the PA calculation\"\n    },\n    \"benchmarkpricingsources\": {\n      \"type\": \"array\",\n      \"description\": \"List of benchmark pricing source for the PA calculation\"\n    },\n    \"useportfoliopricingsourcesforbenchmark\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use portfolio pricing sources for benchmark\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-calculation-data-sources-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PACalculationDataSources
---
