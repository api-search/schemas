---
description: Returns Coverage Response of the requested ticker with unique isocode within a date range
layout: schema
name: coverageTickHistory
properties_list:
- description: a unique ticker given to a company
  name: ticker
  type: string
- description: FactSet specific exchange code.
  name: factsetExchangeCode
  type: string
- description: The date for (or from which) the coverage is required.
  name: startDate
  type: string
- description: This specifies the latest traded date from tick history.
  name: latestTradeDate
  type: string
- description: Name of the firm
  name: companyName
  type: string
- description: returns the ISIN of the requested company
  name: isin
  type: string
- description: Represents 3 digit ISO code for the currency
  name: currency
  type: string
- description: the last traded exhange code from tick history
  name: lastExchangeCode
  type: string
- description: the last traded exchange name from tick history
  name: lastExchangeName
  type: string
- description: the primary ticker iso
  name: primaryTickerExchange
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-coverage-tick-history-schema.json
slug: factset-tick-history-coverage-tick-history
source_filename: factset-tick-history-coverage-tick-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"coverageTickHistory\",\n  \"type\": \"object\",\n  \"description\": \"Returns Coverage Response of the requested ticker with unique isocode within a date range\",\n  \"properties\": {\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"a unique ticker given to a company\"\n    },\n    \"factsetExchangeCode\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet specific exchange code.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date for (or from which) the coverage is required. \"\n    },\n    \"latestTradeDate\": {\n      \"type\": \"string\",\n      \"description\": \"This specifies the latest traded date from tick history.\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the firm\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"\
  returns the ISIN of the requested company \"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Represents 3 digit ISO code for the currency\"\n    },\n    \"lastExchangeCode\": {\n      \"type\": \"string\",\n      \"description\": \"the last traded exhange code from tick history\"\n    },\n    \"lastExchangeName\": {\n      \"type\": \"string\",\n      \"description\": \"the last traded exchange name from tick history\"\n    },\n    \"primaryTickerExchange\": {\n      \"type\": \"string\",\n      \"description\": \"the primary ticker iso\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-coverage-tick-history-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: coverageTickHistory
---
