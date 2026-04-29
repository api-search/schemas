---
description: ''
layout: schema
name: AntiPattern
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: symptoms
  type: array
- description: ''
  name: causes
  type: array
- description: ''
  name: refactoredSolution
  type: string
- description: ''
  name: relatedPatterns
  type: array
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
schema_file: json-schema/architectural-design-patterns-api-anti-pattern-schema.json
slug: architectural-design-patterns-api-anti-pattern
source_filename: architectural-design-patterns-api-anti-pattern-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-anti-pattern-schema.json\",\n  \"title\": \"AntiPattern\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"symptoms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"causes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"refactoredSolution\": {\n      \"type\": \"string\"\n    },\n    \"relatedPatterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-anti-pattern-schema.json
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
title: AntiPattern
---
