---
description: ''
layout: schema
name: PubIdentifier
properties_list:
- description: User's FactSet account path OR benchmark.
  name: id
  type: string
- description: Holdings Mode can be B&H, TBR, OMS or EXT.
  name: holdingsmode
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-publisher-pub-identifier-schema.json
slug: factset-publisher-pub-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PubIdentifier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User's FactSet account path OR benchmark.\"\n    },\n    \"holdingsmode\": {\n      \"type\": \"string\",\n      \"description\": \"Holdings Mode can be B&H, TBR, OMS or EXT.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-publisher-pub-identifier-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PubIdentifier
---
