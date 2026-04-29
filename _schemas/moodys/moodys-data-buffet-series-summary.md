---
description: Summary metadata for a series returned in search results.
layout: schema
name: SeriesSummary
properties_list:
- description: The unique series mnemonic identifier.
  name: mnemonic
  type: string
- description: Human-readable description of the series.
  name: description
  type: string
- description: Native frequency of the series.
  name: frequency
  type: string
- description: The original data source.
  name: source
  type: string
- description: Geographic area covered by the series.
  name: geography
  type: string
- description: Data category classification.
  name: category
  type: string
- description: Earliest available observation date.
  name: startDate
  type: string
- description: Latest available observation or forecast date.
  name: endDate
  type: string
- description: Whether the series includes forecast data from Moody's Analytics models.
  name: hasForecast
  type: boolean
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-series-summary-schema.json
slug: moodys-data-buffet-series-summary
source_filename: moodys-data-buffet-series-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SeriesSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary metadata for a series returned in search results.\",\n  \"properties\": {\n    \"mnemonic\": {\n      \"type\": \"string\",\n      \"description\": \"The unique series mnemonic identifier.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the series.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Native frequency of the series.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The original data source.\"\n    },\n    \"geography\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic area covered by the series.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Data category classification.\"\n    },\n    \"startDate\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Earliest available observation date.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"Latest available observation or forecast date.\"\n    },\n    \"hasForecast\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the series includes forecast data from Moody's Analytics models.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-series-summary-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: SeriesSummary
---
