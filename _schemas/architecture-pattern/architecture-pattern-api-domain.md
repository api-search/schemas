---
description: ''
layout: schema
name: Domain
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
  name: patternCount
  type: integer
- description: ''
  name: subdomains
  type: array
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-domain-schema.json
slug: architecture-pattern-api-domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-domain-schema.json\",\n  \"title\": \"Domain\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"patternCount\": {\n      \"type\": \"integer\"\n    },\n    \"subdomains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-domain-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: Domain
---
