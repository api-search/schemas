---
description: ''
layout: schema
name: annualizedDividendsObject
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: FactSet identifier that uniquely identifies the Event.
  name: eventId
  type: string
- description: Effective Date or Ex-Date of Annualized Dividend in YYYY-MM-DD format.
  name: effectiveDate
  type: string
- description: Annualized Dividend value in the trading currency. The value is adjusted for splits
  name: iadDefTradingAdj
  type: number
- description: 'Currency ISO code associated with the annualized dividends.For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-annualized-dividends-object-schema.json
slug: factset-global-prices-annualized-dividends-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"annualizedDividendsObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet identifier that uniquely identifies the Event.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective Date or Ex-Date of Annualized Dividend in YYYY-MM-DD\
  \ format.\"\n    },\n    \"iadDefTradingAdj\": {\n      \"type\": \"number\",\n      \"description\": \"Annualized Dividend value in the trading currency. The value is adjusted for splits\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code associated with the annualized dividends.For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-annualized-dividends-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: annualizedDividendsObject
---
