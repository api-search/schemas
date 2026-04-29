---
description: ''
layout: schema
name: OptimizerTradesList
properties_list:
- description: Identifier type
  name: identifierType
  type: string
- description: Include cash
  name: includeCash
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-northfield-portfolio-optimizer-optimizer-trades-list-schema.json
slug: factset-northfield-portfolio-optimizer-optimizer-trades-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OptimizerTradesList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifierType\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier type\"\n    },\n    \"includeCash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Include cash\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-northfield-portfolio-optimizer-optimizer-trades-list-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: OptimizerTradesList
---
