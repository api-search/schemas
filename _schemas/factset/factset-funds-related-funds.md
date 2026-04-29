---
description: ''
layout: schema
name: relatedFunds
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The first related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).
  name: relatedFundIdOne
  type: string
- description: The second related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).
  name: relatedFundIdTwo
  type: string
- description: The third related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).
  name: relatedFundIdThree
  type: string
- description: The fourth related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).
  name: relatedFundIdFour
  type: string
- description: The fifth related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).
  name: relatedFundIdFive
  type: string
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-related-funds-schema.json
slug: factset-funds-related-funds
source_filename: factset-funds-related-funds-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"relatedFunds\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"relatedFundIdOne\": {\n      \"type\": \"string\",\n      \"description\": \"The first related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).\"\n    },\n    \"relatedFundIdTwo\": {\n      \"type\": \"string\",\n      \"description\": \"The second related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).\"\n    },\n    \"relatedFundIdThree\": {\n      \"type\": \"string\",\n      \"description\": \"The third related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).\"\n    },\n\
  \    \"relatedFundIdFour\": {\n      \"type\": \"string\",\n      \"description\": \"The fourth related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).\"\n    },\n    \"relatedFundIdFive\": {\n      \"type\": \"string\",\n      \"description\": \"The fifth related fund to the requestedId returned as a FactSet Permanent Security Identifier (XXXXXX-S).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-related-funds-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: relatedFunds
---
