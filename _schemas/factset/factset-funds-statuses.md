---
description: ''
layout: schema
name: statuses
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: Binary flag to indicate whether the fund is currently active, where 1 is active and 0 is inactive.
  name: activeFlag
  type: integer
- description: Returns a binary indicator of whether the specified share class is currently active, where 1 is active and 0 is inactive.
  name: shrClassActiveFlag
  type: integer
- description: Returns a binary indicator of whether the specified fund is available in the FactSet Funds Database (FFD).
  name: isonFFD
  type: integer
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-statuses-schema.json
slug: factset-funds-statuses
source_filename: factset-funds-statuses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"statuses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"activeFlag\": {\n      \"type\": \"integer\",\n      \"description\": \"Binary flag to indicate whether the fund is currently active, where 1 is active and 0 is inactive.\"\n    },\n    \"shrClassActiveFlag\": {\n      \"type\": \"integer\",\n      \"description\": \"Returns a binary indicator of whether the specified share class is currently active, where 1 is active and 0 is inactive.\"\n    },\n    \"isonFFD\": {\n      \"type\": \"integer\",\n      \"description\": \"Returns a binary indicator of whether the specified fund is available in the FactSet Funds Database (FFD).\"\n    },\n   \
  \ \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-statuses-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: statuses
---
