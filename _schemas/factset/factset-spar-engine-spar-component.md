---
description: ''
layout: schema
name: SPARComponent
properties_list:
- description: Component identifier.
  name: id
  type: string
- description: List of accounts in SPAR document.
  name: accounts
  type: array
- description: CurrencyCode in SPAR document.
  name: currencyIsoCode
  type: string
- description: The path to the document
  name: path
  type: string
- description: Component name.
  name: name
  type: string
- description: Component category.
  name: category
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-spar-engine-spar-component-schema.json
slug: factset-spar-engine-spar-component
source_filename: factset-spar-engine-spar-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SPARComponent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Component identifier.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts in SPAR document.\"\n    },\n    \"currencyIsoCode\": {\n      \"type\": \"string\",\n      \"description\": \"CurrencyCode in SPAR document.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the document\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Component name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Component category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-spar-engine-spar-component-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SPARComponent
---
