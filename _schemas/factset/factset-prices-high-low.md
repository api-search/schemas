---
description: ''
layout: schema
name: highLow
properties_list:
- description: Date of last split for which prices have been adjusted.
  name: adjDate
  type: string
- description: Specific reference date for the period expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: The period of measure requested using the period query parameter.
  name: period
  type: string
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: High price over the period requested. This can represent the intra-day or closing price depending on the priceType requested. By default the price is as of closing in local trading currency, split adj
  name: priceHigh
  type: number
- description: Low price over the period requested. This can represent the intra-day or closing price depending on the priceType requested. By default the price is as of closing in local trading currency, split adju
  name: priceLow
  type: number
- description: Date in which the highest price occurred over the requested period for the given id expressed in YYYY-MM-DD format.
  name: priceHighDate
  type: string
- description: Date in which the lowest price occurred over the requested period for the given id expressed in YYYY-MM-DD format.
  name: priceLowDate
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-high-low-schema.json
slug: factset-prices-high-low
source_filename: factset-prices-high-low-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"highLow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adjDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of last split for which prices have been adjusted.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Specific reference date for the period expressed in YYYY-MM-DD format.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"The period of measure requested using the period query parameter.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent\
  \ identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"priceHigh\": {\n      \"type\": \"number\",\n      \"description\": \"High price over the period requested. This can represent the intra-day or closing price depending on the priceType requested. By default the price is as of closing in local trading currency, split adjusted and not spinoff adjusted.\"\n    },\n    \"priceLow\": {\n      \"type\": \"number\",\n      \"description\": \"Low price over the period requested. This can represent the intra-day or closing price depending on the priceType requested. By default the price is as of closing in local trading currency, split adjusted and not spinoff adjusted.\"\n    },\n    \"priceHighDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date in which the highest price occurred over the requested period  for the given id expressed in YYYY-MM-DD format.\"\n    },\n    \"priceLowDate\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Date in which the lowest price occurred over the requested period for the given id expressed in YYYY-MM-DD format.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-high-low-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: highLow
---
