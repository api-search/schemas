---
description: ''
layout: schema
name: return
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: End date of the return. Date in YYYY-MM-DD format. Depending on Frequency and Calendar settings, this could represent the entire return period requested.
  name: date
  type: string
- description: Date of last split for which return has been adjusted.
  name: adjDate
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: The simple or compound return for the requested `frequency` and/or `rolling_period`. Depending on the input parameters the return will adjust accordingly. If you simply use `frequency` and no `rolling
  name: totalReturn
  type: number
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-return-schema.json
slug: factset-prices-return
source_filename: factset-prices-return-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"return\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"End date of the return. Date in YYYY-MM-DD format. Depending on Frequency and Calendar settings, this could represent the entire return period requested.\"\n    },\n    \"adjDate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Date of last split for which return has been adjusted.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"totalReturn\": {\n      \"type\": \"number\",\n      \"description\": \"The simple or compound return for the requested `frequency` and/or `rolling_period`. Depending on the input parameters the return will adjust accordingly. If you simply use `frequency` and no `rolling_period`, the return value will represent the frequency period. If you use `rolling_period`, the values will be returned in actual period ends (e.g. actual month, actual week, daily, etc.). General Return Calculation Details found on [Online Assistant Page #8748](https://oa.apps.factset.com/pages/8748)\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-return-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: return
---
