---
description: ''
layout: schema
name: Relationship
properties_list:
- description: Relationship identifier
  name: id
  type: string
- description: ArchiMate relationship type
  name: type
  type: string
- description: Source element identifier
  name: sourceId
  type: string
- description: Target element identifier
  name: targetId
  type: string
- description: Optional relationship label
  name: label
  type: string
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-relationship-schema.json
slug: archimate-model-exchange-api-relationship
source_filename: archimate-model-exchange-api-relationship-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Relationship identifier\",\n      \"example\": \"rel-001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"ArchiMate relationship type\",\n      \"enum\": [\n        \"Association\",\n        \"Composition\",\n        \"Aggregation\",\n        \"Assignment\",\n        \"Realization\",\n        \"Serving\",\n        \"Access\",\n        \"Influence\",\n        \"Triggering\",\n        \"Flow\",\n        \"Specialization\"\n      ],\n      \"example\": \"Assignment\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"Source element identifier\",\n      \"example\": \"elem-001\"\n    },\n    \"targetId\": {\n      \"type\": \"string\",\n      \"description\": \"Target element identifier\",\n      \"example\": \"elem-002\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Optional relationship label\",\n      \"example\": \"supports\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-relationship-schema.json\",\n  \"title\": \"Relationship\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-relationship-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: Relationship
---
