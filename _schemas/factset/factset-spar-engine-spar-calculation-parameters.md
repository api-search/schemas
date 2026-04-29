---
description: ''
layout: schema
name: SPARCalculationParameters
properties_list:
- description: The SPAR Engine component identifier to analyze.
  name: componentid
  type: string
- description: List of accounts for SPAR calculation.
  name: accounts
  type: array
- description: Currency ISO code for calculation.
  name: currencyisocode
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-spar-engine-spar-calculation-parameters-schema.json
slug: factset-spar-engine-spar-calculation-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SPARCalculationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentid\": {\n      \"type\": \"string\",\n      \"description\": \"The SPAR Engine component identifier to analyze.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts for SPAR calculation.\"\n    },\n    \"currencyisocode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code for calculation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-spar-engine-spar-calculation-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SPARCalculationParameters
---
