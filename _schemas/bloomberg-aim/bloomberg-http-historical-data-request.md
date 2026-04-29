---
description: ''
layout: schema
name: HistoricalDataRequest
properties_list:
- description: List of security identifiers
  name: securities
  type: array
- description: List of Bloomberg field mnemonics
  name: fields
  type: array
- description: Start date in YYYYMMDD format
  name: startDate
  type: string
- description: End date in YYYYMMDD format
  name: endDate
  type: string
- description: ''
  name: periodicitySelection
  type: string
- description: ''
  name: periodicityAdjustment
  type: string
- description: Three-letter currency code for cross-currency conversion
  name: currency
  type: string
- description: ''
  name: overrides
  type: array
- description: ''
  name: nonTradingDayFillOption
  type: string
- description: ''
  name: nonTradingDayFillMethod
  type: string
- description: ''
  name: adjustmentNormal
  type: boolean
- description: ''
  name: adjustmentAbnormal
  type: boolean
- description: ''
  name: adjustmentSplit
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-historical-data-request-schema.json
slug: bloomberg-http-historical-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HistoricalDataRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securities\": {\n      \"type\": \"array\",\n      \"description\": \"List of security identifiers\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of Bloomberg field mnemonics\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date in YYYYMMDD format\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"End date in YYYYMMDD format\"\n    },\n    \"periodicitySelection\": {\n      \"type\": \"string\"\n    },\n    \"periodicityAdjustment\": {\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter currency code for cross-currency conversion\"\n    },\n    \"overrides\": {\n      \"type\": \"array\"\n    },\n    \"nonTradingDayFillOption\"\
  : {\n      \"type\": \"string\"\n    },\n    \"nonTradingDayFillMethod\": {\n      \"type\": \"string\"\n    },\n    \"adjustmentNormal\": {\n      \"type\": \"boolean\"\n    },\n    \"adjustmentAbnormal\": {\n      \"type\": \"boolean\"\n    },\n    \"adjustmentSplit\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-historical-data-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: HistoricalDataRequest
---
