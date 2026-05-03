---
description: Schema for a commodity price assessment data point from the S&P Global Commodity Insights API
layout: schema
name: S&P Global Commodity Market Data Point
properties_list:
- description: Commodity symbol code (Platts code)
  name: symbol
  type: string
- description: Assessment date
  name: assessDate
  type: string
- description: Assessment value
  name: value
  type: number
- description: Unit of measure
  name: uom
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Buy/Ask/Trade/End-of-day indicator
  name: bate
  type: string
- description: Last modification timestamp
  name: modDate
  type: string
provider_name: S&P Global
provider_slug: s-and-p-global
schema_file: json-schema/s-and-p-global-market-data-point-schema.json
slug: s-and-p-global-market-data-point
source_filename: s-and-p-global-market-data-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/json-schema/s-and-p-global-market-data-point-schema.json\",\n  \"title\": \"S&P Global Commodity Market Data Point\",\n  \"description\": \"Schema for a commodity price assessment data point from the S&P Global Commodity Insights API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity symbol code (Platts code)\",\n      \"example\": \"PCAAS00\"\n    },\n    \"assessDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Assessment date\",\n      \"example\": \"2024-12-01\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Assessment value\",\n      \"example\": 72.45\n    },\n    \"uom\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Unit of measure\",\n      \"example\": \"USD/BBL\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"example\": \"USD\"\n    },\n    \"bate\": {\n      \"type\": \"string\",\n      \"description\": \"Buy/Ask/Trade/End-of-day indicator\",\n      \"enum\": [\"B\", \"A\", \"T\", \"C\"],\n      \"example\": \"C\"\n    },\n    \"modDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"required\": [\"symbol\", \"assessDate\", \"value\", \"uom\", \"currency\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/json-schema/s-and-p-global-market-data-point-schema.json
tags:
- Financial Data
- Credit Ratings
- Market Intelligence
- Commodity Insights
- Energy Markets
- Capital Markets
- Fortune 500
title: S&P Global Commodity Market Data Point
---
