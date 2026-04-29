---
description: ''
layout: schema
name: price
properties_list:
- description: FactSet Permanent Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R) or a -L Suffix (XXXXXX-L).
  name: fsymId
  type: string
- description: Ending date for the period expressed in YYYY-MM-DD format.
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
schema_file: json-schema/factset-global-prices-price-schema.json
slug: factset-global-prices-price
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"price\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R) or a -L Suffix (XXXXXX-L).\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Ending date for the period expressed in YYYY-MM-DD format.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-price-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: price
---
