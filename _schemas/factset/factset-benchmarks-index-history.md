---
description: ''
layout: schema
name: indexHistory
properties_list:
- description: Requested Identifier. Must be a valid Benchmark Identifier recognized by FactSet.
  name: fsymId
  type: string
- description: The respective date for values as of the date requested in YYYY-MM-DD format.
  name: date
  type: string
- description: Proper Name of Index.
  name: name
  type: string
- description: The total number of constituents as of the date requested.
  name: constituentNumber
  type: integer
- description: Currency Code used in adjustments. If no Currency was requested, the service will default to LOCAL ('LOC').
  name: currency
  type: string
- description: Index Level Market Capitalization as of the date requested expressed in millions.
  name: marketValue
  type: number
- description: Index Level Price
  name: price
  type: number
- description: Index Level Price Percent Change
  name: priceReturnPercent
  type: number
- description: Index Level Total Return Amount
  name: totalReturnLevel
  type: number
- description: Index Level Total Return Percent Change
  name: totalReturnPercent
  type: number
- description: The requested Return Type - GROSS or NET
  name: returnType
  type: string
- description: The requested Hedge Type - HEDGED or UNHEDGED
  name: hedgeType
  type: string
- description: Benchmark Identifier specified in the request
  name: requestId
  type: string
- description: This field will always return the date of the data that was actually returned.
  name: observationDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-index-history-schema.json
slug: factset-benchmarks-index-history
source_filename: factset-benchmarks-index-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"indexHistory\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Requested Identifier. Must be a valid Benchmark Identifier recognized by FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The respective date for values as of the date requested in YYYY-MM-DD format.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Proper Name of Index.\"\n    },\n    \"constituentNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of constituents as of the date requested.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency Code used in adjustments. If no Currency was requested, the service will default to LOCAL ('LOC').\"\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"\
  description\": \"Index Level Market Capitalization as of the date requested expressed in millions.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price\"\n    },\n    \"priceReturnPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price Percent Change\"\n    },\n    \"totalReturnLevel\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return Amount\"\n    },\n    \"totalReturnPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return Percent Change\"\n    },\n    \"returnType\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Return Type - GROSS or NET\"\n    },\n    \"hedgeType\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Hedge Type - HEDGED or UNHEDGED\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Identifier specified in the request\"\n    },\n  \
  \  \"observationDate\": {\n      \"type\": \"string\",\n      \"description\": \"This field will always return the date of the data that was actually returned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-index-history-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: indexHistory
---
