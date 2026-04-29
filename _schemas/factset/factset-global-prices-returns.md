---
description: ''
layout: schema
name: returns
properties_list:
- description: FactSet Permanent Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R) or a -L Suffix (XXXXXX-L).
  name: fsymId
  type: string
- description: Returns the data for the given input parameters.
  name: totalReturn
  type: number
- description: End date of the return. Date in YYYY-MM-DD format. Depending on Frequency and Calendar settings, this could represent the entire return period requested.
  name: date
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-returns-schema.json
slug: factset-global-prices-returns
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"returns\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R) or a -L Suffix (XXXXXX-L).\"\n    },\n    \"totalReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the data for the given input parameters.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"End date of the return. Date in YYYY-MM-DD format. Depending on Frequency and Calendar settings, this could represent the entire return period requested.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-returns-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: returns
---
