---
description: ''
layout: schema
name: entityFocus
properties_list:
- description: Company identifier used in request.
  name: requestId
  type: string
- description: FactSet Company identifier being classified.
  name: fsymId
  type: string
- description: First date of the classification.
  name: firstDate
  type: string
- description: Date when the classification became no longer valid.
  name: lastDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-rbics-entity-focus-schema.json
slug: factset-rbics-entity-focus
source_filename: factset-rbics-entity-focus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"entityFocus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Company identifier used in request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Company identifier being classified.\"\n    },\n    \"firstDate\": {\n      \"type\": \"string\",\n      \"description\": \"First date of the classification.\"\n    },\n    \"lastDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date when the classification became no longer valid.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-rbics-entity-focus-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: entityFocus
---
