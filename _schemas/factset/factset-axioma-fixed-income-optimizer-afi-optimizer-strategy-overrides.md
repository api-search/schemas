---
description: ''
layout: schema
name: AFIOptimizerStrategyOverrides
properties_list:
- description: Objective
  name: objective
  type: string
- description: Tax
  name: tax
  type: string
- description: List of constraints
  name: constraints
  type: object
- description: Alpha
  name: alpha
  type: string
- description: Transaction cost
  name: transactionCost
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-axioma-fixed-income-optimizer-afi-optimizer-strategy-overrides-schema.json
slug: factset-axioma-fixed-income-optimizer-afi-optimizer-strategy-overrides
source_filename: factset-axioma-fixed-income-optimizer-afi-optimizer-strategy-overrides-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AFIOptimizerStrategyOverrides\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objective\": {\n      \"type\": \"string\",\n      \"description\": \"Objective\"\n    },\n    \"tax\": {\n      \"type\": \"string\",\n      \"description\": \"Tax\"\n    },\n    \"constraints\": {\n      \"type\": \"object\",\n      \"description\": \"List of constraints\"\n    },\n    \"alpha\": {\n      \"type\": \"string\",\n      \"description\": \"Alpha\"\n    },\n    \"transactionCost\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction cost\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-axioma-fixed-income-optimizer-afi-optimizer-strategy-overrides-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: AFIOptimizerStrategyOverrides
---
