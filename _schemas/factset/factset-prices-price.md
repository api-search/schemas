---
description: ''
layout: schema
name: price
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: Ending date for the period expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: Date of last split for which prices and volume have been adjusted. Use /factset-prices/v#/splits endpoint for details regarding the split.
  name: adjDate
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: Closing Price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.
  name: price
  type: number
- description: Open price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.
  name: priceOpen
  type: number
- description: High closing price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.
  name: priceHigh
  type: number
- description: Low closing price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.
  name: priceLow
  type: number
- description: Returns the cumulative volume over dates requested. Data is returned in thousands.
  name: volume
  type: number
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-price-schema.json
slug: factset-prices-price
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"price\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Ending date for the period expressed in YYYY-MM-DD format.\"\n    },\n    \"adjDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of last split for which prices and volume have been adjusted. Use /factset-prices/v#/splits\
  \ endpoint for details regarding the split.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Closing Price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.\"\n    },\n    \"priceOpen\": {\n      \"type\": \"number\",\n      \"description\": \"Open price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted. Prices updated nightly at approximately at 9pm ET.\"\n    },\n    \"priceHigh\": {\n      \"type\": \"number\",\n      \"description\": \"High closing price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff\
  \ adjusted.  Prices updated nightly at approximately at 9pm ET.\"\n    },\n    \"priceLow\": {\n      \"type\": \"number\",\n      \"description\": \"Low closing price as of the date(s) requested. By default the price is in local trading currency, split adjusted and not spinoff adjusted.  Prices updated nightly at approximately at 9pm ET.\"\n    },\n    \"volume\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the cumulative volume over dates requested. Data is returned in thousands.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-price-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: price
---
