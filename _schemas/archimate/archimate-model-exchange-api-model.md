---
description: ''
layout: schema
name: Model
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
- description: Model creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-model-schema.json
slug: archimate-model-exchange-api-model
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier\",\n      \"example\": \"model-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model name\",\n      \"example\": \"Enterprise Architecture Baseline\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Model version\",\n      \"example\": \"2025.1\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ArchiMate language version\",\n      \"example\": \"ArchiMate 3.2\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Model creation timestamp\",\n      \"example\": \"2026-01-15T10:00:00Z\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\",\n      \"example\": \"2026-04-19T10:00:00Z\"\
  \n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-schema.json\",\n  \"title\": \"Model\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-model-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: Model
---
