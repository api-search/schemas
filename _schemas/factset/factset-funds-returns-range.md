---
description: ''
layout: schema
name: returnsRange
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The Return calculated between two dates. The return type is determined by including or excluding dividends through the dividendAdjust parameter.
  name: return
  type: number
- description: The start date of the return in YYYY-MM-DD format. *NOTE - the startDate cannot be less than the `priceFirstDate` which can be accessed in the /summary endpoint.
  name: returnStartDate
  type: string
- description: The end date of the return in YYYY-MM-DD format. The start date of the return in YYYY-MM-DD format. *NOTE - the startDate cannot be less than the `priceFirstDate` which can be accessed in the /summary
  name: returnEndDate
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-returns-range-schema.json
slug: factset-funds-returns-range
source_filename: factset-funds-returns-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"returnsRange\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"return\": {\n      \"type\": \"number\",\n      \"description\": \"The Return calculated between two dates. The return type is determined by including or excluding dividends through the dividendAdjust parameter.\"\n    },\n    \"returnStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the return in YYYY-MM-DD format. *NOTE - the startDate cannot be less than the `priceFirstDate` which can be accessed in the /summary endpoint.\"\n    },\n    \"returnEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"The end date of the return in YYYY-MM-DD\
  \ format. The start date of the return in YYYY-MM-DD format. *NOTE - the startDate cannot be less than the `priceFirstDate` which can be accessed in the /summary endpoint.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-returns-range-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: returnsRange
---
