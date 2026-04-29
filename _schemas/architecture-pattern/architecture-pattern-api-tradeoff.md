---
description: ''
layout: schema
name: Tradeoff
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: patternId
  type: string
- description: ''
  name: dimension
  type: string
- description: ''
  name: benefit
  type: string
- description: ''
  name: drawback
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: notes
  type: string
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-tradeoff-schema.json
slug: architecture-pattern-api-tradeoff
source_filename: architecture-pattern-api-tradeoff-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-tradeoff-schema.json\",\n  \"title\": \"Tradeoff\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"patternId\": {\n      \"type\": \"string\"\n    },\n    \"dimension\": {\n      \"type\": \"string\"\n    },\n    \"benefit\": {\n      \"type\": \"string\"\n    },\n    \"drawback\": {\n      \"type\": \"string\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\"\n      ]\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-tradeoff-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: Tradeoff
---
