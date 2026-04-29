---
description: ''
layout: schema
name: PACalculationParameters
properties_list:
- description: The PA Engine component identifier to analyze.
  name: componentid
  type: string
- description: List of accounts.
  name: accounts
  type: array
- description: List of benchmarks.
  name: benchmarks
  type: array
- description: List of groupings for the PA calculation. This will take precedence over the groupings saved in the PA document.
  name: groups
  type: array
- description: Currency ISO code for calculation.
  name: currencyisocode
  type: string
- description: List of columns for the PA calculation. This will take precedence over the columns saved in the PA document.
  name: columns
  type: array
- description: Component detail type for the PA component. It can be GROUPS or GROUPSALL or TOTALS or SECURITIES.
  name: componentdetail
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-pa-calculation-parameters-schema.json
slug: factset-pa-engine-pa-calculation-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PACalculationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentid\": {\n      \"type\": \"string\",\n      \"description\": \"The PA Engine component identifier to analyze.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts.\"\n    },\n    \"benchmarks\": {\n      \"type\": \"array\",\n      \"description\": \"List of benchmarks.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"List of groupings for the PA calculation. This will take precedence over the groupings saved in the PA document.\"\n    },\n    \"currencyisocode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code for calculation.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of columns for the PA calculation. This will take precedence over the columns saved\
  \ in the PA document.\"\n    },\n    \"componentdetail\": {\n      \"type\": \"string\",\n      \"description\": \"Component detail type for the PA component. It can be GROUPS or GROUPSALL or TOTALS or SECURITIES.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-calculation-parameters-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PACalculationParameters
---
