---
description: ''
layout: schema
name: Optimization
properties_list:
- description: Risk model date
  name: riskModelDate
  type: string
- description: Backtest date
  name: backtestDate
  type: string
- description: Cash flow
  name: cashflow
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-optimizer-optimization-schema.json
slug: factset-portfolio-optimizer-optimization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Optimization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"riskModelDate\": {\n      \"type\": \"string\",\n      \"description\": \"Risk model date\"\n    },\n    \"backtestDate\": {\n      \"type\": \"string\",\n      \"description\": \"Backtest date\"\n    },\n    \"cashflow\": {\n      \"type\": \"string\",\n      \"description\": \"Cash flow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-optimizer-optimization-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Optimization
---
