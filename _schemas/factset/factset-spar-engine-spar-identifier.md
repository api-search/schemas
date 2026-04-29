---
description: The account/benchmark parameter for SPAR calculation.
layout: schema
name: SPARIdentifier
properties_list:
- description: User's FactSet account OR benchmark id.
  name: id
  type: string
- description: Benchmark return type.
  name: returntype
  type: string
- description: Benchmark prefix.
  name: prefix
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-spar-engine-spar-identifier-schema.json
slug: factset-spar-engine-spar-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SPARIdentifier\",\n  \"type\": \"object\",\n  \"description\": \"The account/benchmark parameter for SPAR calculation.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User's FactSet account OR benchmark id.\"\n    },\n    \"returntype\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark return type.\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark prefix.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-spar-engine-spar-identifier-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SPARIdentifier
---
