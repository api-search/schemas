---
description: ''
layout: schema
name: ModelDetail
properties_list:
- description: Unique model identifier
  name: id
  type: string
- description: Model name
  name: name
  type: string
- description: Model version
  name: version
  type: string
- description: ArchiMate language version
  name: language
  type: string
- description: Number of elements in the model
  name: elementCount
  type: integer
- description: Number of relationships in the model
  name: relationshipCount
  type: integer
- description: Number of views in the model
  name: viewCount
  type: integer
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-model-detail-schema.json
slug: archimate-model-exchange-api-model-detail
source_filename: archimate-model-exchange-api-model-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier\",\n      \"example\": \"model-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model name\",\n      \"example\": \"Enterprise Architecture Baseline\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Model version\",\n      \"example\": \"2025.1\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ArchiMate language version\",\n      \"example\": \"ArchiMate 3.2\"\n    },\n    \"elementCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of elements in the model\",\n      \"example\": 85\n    },\n    \"relationshipCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of relationships in the model\",\n      \"example\": 120\n    },\n    \"viewCount\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Number of views in the model\",\n      \"example\": 12\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-detail-schema.json\",\n  \"title\": \"ModelDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-detail-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: ModelDetail
---
