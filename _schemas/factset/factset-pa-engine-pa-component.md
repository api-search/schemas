---
description: ''
layout: schema
name: PAComponent
properties_list:
- description: Component identifier.
  name: id
  type: string
- description: List of accounts saved in the PA document.
  name: accounts
  type: array
- description: List of benchmarks saved in the PA document.
  name: benchmarks
  type: array
- description: ''
  name: currencyisocode
  type: string
- description: Is the component type snapshot or subperiod.
  name: snapshot
  type: boolean
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
schema_file: json-schema/factset-pa-engine-pa-component-schema.json
slug: factset-pa-engine-pa-component
source_filename: factset-pa-engine-pa-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PAComponent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Component identifier.\"\n    },\n    \"accounts\": {\n      \"type\": \"array\",\n      \"description\": \"List of accounts saved in the PA document.\"\n    },\n    \"benchmarks\": {\n      \"type\": \"array\",\n      \"description\": \"List of benchmarks saved in the PA document.\"\n    },\n    \"currencyisocode\": {\n      \"type\": \"string\"\n    },\n    \"snapshot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Is the component type snapshot or subperiod.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the document\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Component name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Component\
  \ category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-component-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PAComponent
---
