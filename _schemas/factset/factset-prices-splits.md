---
description: ''
layout: schema
name: splits
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: Ex-Date of the split expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: Split adjustment factor for n splits ago. A 2-for-1 split returns .50, the number you would multiply the stock price by to adjust for the split.
  name: splitFactor
  type: number
- description: Description for the type of split or spin off.
  name: splitComment
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-splits-schema.json
slug: factset-prices-splits
source_filename: factset-prices-splits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"splits\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Ex-Date of the split expressed in YYYY-MM-DD format.\"\n    },\n    \"splitFactor\": {\n      \"type\": \"number\",\n      \"description\": \"Split adjustment factor for n splits ago. A 2-for-1 split returns .50, the number you would\
  \ multiply the stock price by to adjust for the split.\"\n    },\n    \"splitComment\": {\n      \"type\": \"string\",\n      \"description\": \"Description for the type of split or spin off.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-splits-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: splits
---
