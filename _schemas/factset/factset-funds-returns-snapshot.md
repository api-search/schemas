---
description: ''
layout: schema
name: returnsSnapshot
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The one-week return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: oneWeek
  type: number
- description: The one-month return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: oneMonth
  type: number
- description: The three-month return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: threeMonth
  type: number
- description: The year-to-date return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: yearToDate
  type: number
- description: The one-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: oneYear
  type: number
- description: The three-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: threeYear
  type: number
- description: The three-year annualized return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: threeYearAnnualized
  type: number
- description: The five-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: fiveYear
  type: number
- description: The five year annualized return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: fiveYearAnnualized
  type: number
- description: The date of the return in YYYY-MM-DD format.
  name: date
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-returns-snapshot-schema.json
slug: factset-funds-returns-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"returnsSnapshot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"oneWeek\": {\n      \"type\": \"number\",\n      \"description\": \"The one-week return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"oneMonth\": {\n      \"type\": \"number\",\n      \"description\": \"The one-month return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"threeMonth\": {\n      \"type\": \"number\",\n      \"description\": \"The three-month return for the requested\
  \ id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"yearToDate\": {\n      \"type\": \"number\",\n      \"description\": \"The year-to-date return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"oneYear\": {\n      \"type\": \"number\",\n      \"description\": \"The one-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"threeYear\": {\n      \"type\": \"number\",\n      \"description\": \"The three-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"threeYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"The three-year annualized return for the requested id\
  \ and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"fiveYear\": {\n      \"type\": \"number\",\n      \"description\": \"The five-year return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"fiveYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"The five year annualized return for the requested id and date. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the return in YYYY-MM-DD format.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-returns-snapshot-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: returnsSnapshot
---
