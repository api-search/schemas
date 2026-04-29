---
description: ''
layout: schema
name: sasbRanks
properties_list:
- description: Date for the period requested expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).
  name: fsymId
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: The specific SASB 'category' the Rank is referring to.
  name: sasbCategory
  type: string
- description: The SASB Rank for the given category in Proper format. |Rank|Industry Percentile Range (%)| ||| |Leader|90 - 100| |Above Average|70 - 89.9| |Average|30 - 69.9| |Below Average|10 - 29.9| |Laggard|0 - 9
  name: sasbRank
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-sasb-ranks-schema.json
slug: factset-esg-sasb-ranks
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sasbRanks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date for the period requested expressed in YYYY-MM-DD format.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"sasbCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The specific SASB 'category' the Rank is referring to.\"\n    },\n    \"sasbRank\": {\n      \"type\": \"string\",\n      \"description\": \"The SASB Rank for the given category in Proper format.\\n  |Rank|Industry Percentile Range (%)|\\n  |||\\n  |Leader|90 - 100|\\n  |Above Average|70 - 89.9|\\n  |Average|30\
  \ - 69.9|\\n  |Below Average|10 - 29.9|\\n  |Laggard|0 - 9.9|\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-sasb-ranks-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: sasbRanks
---
