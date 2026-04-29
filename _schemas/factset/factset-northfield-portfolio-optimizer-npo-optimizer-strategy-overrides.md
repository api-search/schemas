---
description: ''
layout: schema
name: NPOOptimizerStrategyOverrides
properties_list:
- description: Objective parameters
  name: objective
  type: object
- description: List of constraints
  name: constraints
  type: array
- description: Tax Can be set to "" for local
  name: tax
  type: string
- description: Transaction cost Can be set to "" for local
  name: transactionCost
  type: string
- description: Alpha
  name: alpha
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-northfield-portfolio-optimizer-npo-optimizer-strategy-overrides-schema.json
slug: factset-northfield-portfolio-optimizer-npo-optimizer-strategy-overrides
source_filename: factset-northfield-portfolio-optimizer-npo-optimizer-strategy-overrides-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NPOOptimizerStrategyOverrides\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objective\": {\n      \"type\": \"object\",\n      \"description\": \"Objective parameters\"\n    },\n    \"constraints\": {\n      \"type\": \"array\",\n      \"description\": \"List of constraints\"\n    },\n    \"tax\": {\n      \"type\": \"string\",\n      \"description\": \"Tax\\r\\nCan be set to \\\"\\\" for local\"\n    },\n    \"transactionCost\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction cost\\r\\nCan be set to \\\"\\\" for local\"\n    },\n    \"alpha\": {\n      \"type\": \"string\",\n      \"description\": \"Alpha\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-northfield-portfolio-optimizer-npo-optimizer-strategy-overrides-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: NPOOptimizerStrategyOverrides
---
