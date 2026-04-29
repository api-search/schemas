---
description: ''
layout: schema
name: InstrumentDto
properties_list:
- description: ''
  name: symbol
  type: string
- description: ''
  name: tickerRegion
  type: string
- description: ''
  name: tickerExchange
  type: string
- description: ''
  name: sedol
  type: string
- description: ''
  name: cusip
  type: string
- description: ''
  name: isin
  type: string
- description: ''
  name: instrumentName
  type: string
- description: ''
  name: identifiers
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-custom-symbols-instrument-dto-schema.json
slug: factset-irn-custom-symbols-instrument-dto
source_filename: factset-irn-custom-symbols-instrument-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstrumentDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\"\n    },\n    \"tickerRegion\": {\n      \"type\": \"string\"\n    },\n    \"tickerExchange\": {\n      \"type\": \"string\"\n    },\n    \"sedol\": {\n      \"type\": \"string\"\n    },\n    \"cusip\": {\n      \"type\": \"string\"\n    },\n    \"isin\": {\n      \"type\": \"string\"\n    },\n    \"instrumentName\": {\n      \"type\": \"string\"\n    },\n    \"identifiers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-custom-symbols-instrument-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: InstrumentDto
---
