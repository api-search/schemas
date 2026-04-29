---
description: ''
layout: schema
name: nonPeriodic
properties_list:
- description: Unique FactSet-generated identifier representing an entity for the current entity identifier (-E)
  name: fsymId
  type: string
- description: Identifier used in `ids`.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-private-markets-non-periodic-schema.json
slug: factset-private-markets-non-periodic
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"nonPeriodic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique FactSet-generated identifier representing an entity for the current entity identifier (-E)\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier used in `ids`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-private-markets-non-periodic-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: nonPeriodic
---
