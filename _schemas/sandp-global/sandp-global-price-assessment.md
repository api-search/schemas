---
description: Schema for a S&P Global Commodity Insights price assessment record, representing a benchmark commodity price as assessed by Platts editors.
layout: schema
name: S&P Global Price Assessment
properties_list:
- description: Platts symbol code uniquely identifying the commodity assessment
  name: symbol
  type: string
- description: The date of the price assessment in ISO 8601 format
  name: assessDate
  type: string
- description: The assessed price value
  name: value
  type: number
- description: Unit of measure for the price
  name: unit
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Timestamp of last modification
  name: modDate
  type: string
- description: Buy/Ask/Trade/Estimate indicator
  name: bate
  type: string
provider_name: S&P Global
provider_slug: sandp-global
schema_file: json-schema/sandp-global-price-assessment-schema.json
slug: sandp-global-price-assessment
source_filename: sandp-global-price-assessment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sandp-global/json-schema/price-assessment.json\",\n  \"title\": \"S&P Global Price Assessment\",\n  \"description\": \"Schema for a S&P Global Commodity Insights price assessment record, representing a benchmark commodity price as assessed by Platts editors.\",\n  \"type\": \"object\",\n  \"required\": [\"symbol\", \"assessDate\", \"value\", \"unit\", \"currency\"],\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Platts symbol code uniquely identifying the commodity assessment\",\n      \"examples\": [\"PCAAS00\", \"AAQZB00\"]\n    },\n    \"assessDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the price assessment in ISO 8601 format\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The assessed\
  \ price value\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure for the price\",\n      \"examples\": [\"BBL\", \"MT\", \"MMBTU\", \"GAL\", \"TON\"]\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code\",\n      \"examples\": [\"USD\", \"EUR\", \"GBP\"]\n    },\n    \"modDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last modification\"\n    },\n    \"bate\": {\n      \"type\": \"string\",\n      \"description\": \"Buy/Ask/Trade/Estimate indicator\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/json-schema/sandp-global-price-assessment-schema.json
tags:
- Financial Data
- Market Intelligence
- Commodity Insights
- Credit Ratings
- Analytics
- Fortune 500
- Enterprise
title: S&P Global Price Assessment
---
