---
description: Redemption Price Data Items for a Fixed Income security.
layout: schema
name: redemptionPrice
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Date of the Redemption Price.
  name: date
  type: string
- description: Redemption Price Category - * **CALL** = Call prices. * **PUT** = Put prices. * **SF** = Sinking Fund prices.
  name: category
  type: string
- description: Sinking Fund minimum amount.
  name: minAmt
  type: number
- description: Redemption price for the category.
  name: price
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-redemption-price-schema.json
slug: factset-terms-and-conditions-redemption-price
source_filename: factset-terms-and-conditions-redemption-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"redemptionPrice\",\n  \"type\": \"object\",\n  \"description\": \"Redemption Price Data Items for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the Redemption Price.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Redemption Price Category -\\n* **CALL** = Call prices.\\n* **PUT** = Put prices.\\n* **SF** = Sinking Fund prices.\\n\"\n    },\n    \"minAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Sinking Fund minimum amount.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Redemption\
  \ price for the category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-redemption-price-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: redemptionPrice
---
