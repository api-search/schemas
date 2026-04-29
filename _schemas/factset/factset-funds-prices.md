---
description: ''
layout: schema
name: prices
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The NAV for the requested share class. NOTE - FactSet Mutual Funds does not use seven-day yields to price money market funds.
  name: price
  type: number
- description: The date of the NAV in YYYY-MM-DD format.
  name: date
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
- description: ISO3 Currency
  name: currency
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-prices-schema.json
slug: factset-funds-prices
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"prices\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"The NAV for the requested share class. NOTE - FactSet Mutual Funds does not use seven-day yields to price money market funds.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the NAV in YYYY-MM-DD format.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO3 Currency\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-prices-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: prices
---
