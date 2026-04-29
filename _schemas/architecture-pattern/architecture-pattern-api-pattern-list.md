---
description: ''
layout: schema
name: PatternList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: patterns
  type: array
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-pattern-list-schema.json
slug: architecture-pattern-api-pattern-list
source_filename: architecture-pattern-api-pattern-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-pattern-list-schema.json\",\n  \"title\": \"PatternList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"patterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"domain\": {},\n          \"description\": {},\n          \"context\": {},\n          \"problem\": {},\n          \"solution\": {},\n          \"resultingContext\": {},\n          \"tags\": {},\n          \"relatedPatterns\": {},\n          \"externalReferences\": {},\n          \"confidence\": {}\n        }\n      }\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-pattern-list-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: PatternList
---
