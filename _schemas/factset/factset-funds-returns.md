---
description: ''
layout: schema
name: returns
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The Return for the requested id and date. Adjusting the frequency of the time-series does not adjust the return calculation, and simply controls the display frequency. The return type is determined by
  name: return
  type: number
- description: The date of the return in YYYY-MM-DD format.
  name: date
  type: string
- description: ISO3 Currency
  name: currency
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-returns-schema.json
slug: factset-funds-returns
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"returns\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"return\": {\n      \"type\": \"number\",\n      \"description\": \"The Return for the requested id and date. Adjusting the frequency of the time-series does not adjust the return calculation, and simply controls the display frequency. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the return in YYYY-MM-DD format.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO3 Currency\"\n    },\n    \"requestId\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-returns-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: returns
---
