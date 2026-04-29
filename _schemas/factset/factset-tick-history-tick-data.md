---
description: Returns Tick History Response.
layout: schema
name: TickData
properties_list:
- description: Timestamp of when request was made
  name: requestTimestamp
  type: string
- description: Timestamp when the file was last updated
  name: updateTimestamp
  type: string
- description: Returns not Authorized Tickers
  name: notAuthorizedTickers
  type: array
- description: Returns invalid Tickers
  name: invalidTickers
  type: array
- description: Contains list of Files
  name: listOfFiles
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-tick-data-schema.json
slug: factset-tick-history-tick-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TickData\",\n  \"type\": \"object\",\n  \"description\": \" Returns Tick History Response.\",\n  \"properties\": {\n    \"requestTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when request was made\"\n    },\n    \"updateTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the file was last updated\"\n    },\n    \"notAuthorizedTickers\": {\n      \"type\": \"array\",\n      \"description\": \"Returns not Authorized Tickers\"\n    },\n    \"invalidTickers\": {\n      \"type\": \"array\",\n      \"description\": \"Returns invalid Tickers\"\n    },\n    \"listOfFiles\": {\n      \"type\": \"array\",\n      \"description\": \"Contains list of Files\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-tick-data-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TickData
---
