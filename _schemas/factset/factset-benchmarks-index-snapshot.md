---
description: ''
layout: schema
name: indexSnapshot
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
- description: Currency Code used in adjustments. If no Currency was requested, the service will default to the local Calendar.
  name: currency
  type: string
- description: Index Level Market Capitalization as of the date requested expressed in millions.
  name: marketValue
  type: number
- description: Index Level Price
  name: price
  type: number
- description: Index Level Price - 1 Day percent change
  name: priceReturnPercent1D
  type: number
- description: Index Level Price - Quarter-to-Date percent change
  name: priceReturnPercentQTD
  type: number
- description: Index Level Price - Year-to-Date percent change
  name: priceReturnPercentYTD
  type: number
- description: Index Level Total Return Amount. (Gross or Net depends on requested returnType)
  name: totalReturnLevel
  type: number
- description: Index Level Total Return - 1 Day percent change. (Gross or Net depends on requested returnType)
  name: totalReturnPercent1D
  type: number
- description: Index Level Total Return - Quarter-to-Date percent change. (Gross or Net depends on requested returnType)
  name: totalReturnPercentQTD
  type: number
- description: Index Level Total Return - Year-to-Date percent change. (Gross or Net depends on requested returnType)
  name: totalReturnPercentYTD
  type: number
- description: The requested Return Type - GROSS or NET
  name: returnType
  type: string
- description: Benchmark Identifier specified in the request
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-index-snapshot-schema.json
slug: factset-benchmarks-index-snapshot
source_filename: factset-benchmarks-index-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"indexSnapshot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Requested Identifier. Must be a valid Benchmark Identifier recognized by FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The respective date for values as of the date requested in YYYY-MM-DD format.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Proper Name of Index.\"\n    },\n    \"constituentNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of constituents as of the date requested.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency Code used in adjustments. If no Currency was requested, the service will default to the local Calendar.\"\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n  \
  \    \"description\": \"Index Level Market Capitalization as of the date requested expressed in millions.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price\"\n    },\n    \"priceReturnPercent1D\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price - 1 Day percent change\"\n    },\n    \"priceReturnPercentQTD\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price - Quarter-to-Date percent change\"\n    },\n    \"priceReturnPercentYTD\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Price - Year-to-Date percent change\"\n    },\n    \"totalReturnLevel\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return Amount. (Gross or Net depends on requested returnType)\"\n    },\n    \"totalReturnPercent1D\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return - 1 Day percent change. (Gross or Net depends on requested returnType)\"\
  \n    },\n    \"totalReturnPercentQTD\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return - Quarter-to-Date percent change. (Gross or Net depends on requested returnType)\"\n    },\n    \"totalReturnPercentYTD\": {\n      \"type\": \"number\",\n      \"description\": \"Index Level Total Return - Year-to-Date percent change. (Gross or Net depends on requested returnType)\"\n    },\n    \"returnType\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Return Type - GROSS or NET\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark Identifier specified in the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-index-snapshot-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: indexSnapshot
---
