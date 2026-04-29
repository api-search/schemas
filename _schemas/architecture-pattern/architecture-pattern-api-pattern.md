---
description: ''
layout: schema
name: Pattern
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: context
  type: string
- description: ''
  name: problem
  type: string
- description: ''
  name: solution
  type: string
- description: ''
  name: resultingContext
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: relatedPatterns
  type: array
- description: ''
  name: externalReferences
  type: array
- description: ''
  name: confidence
  type: string
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-pattern-schema.json
slug: architecture-pattern-api-pattern
source_filename: architecture-pattern-api-pattern-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-pattern-schema.json\",\n  \"title\": \"Pattern\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"context\": {\n      \"type\": \"string\"\n    },\n    \"problem\": {\n      \"type\": \"string\"\n    },\n    \"solution\": {\n      \"type\": \"string\"\n    },\n    \"resultingContext\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relatedPatterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"externalReferences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"confidence\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"proven\",\n        \"candidate\",\n        \"experimental\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-pattern-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: Pattern
---
