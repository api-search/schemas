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
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: problem
  type: string
- description: ''
  name: solution
  type: string
- description: ''
  name: consequences
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: relatedPatterns
  type: array
- description: ''
  name: applicability
  type: string
- description: ''
  name: knownUses
  type: array
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
schema_file: json-schema/architectural-design-patterns-api-pattern-schema.json
slug: architectural-design-patterns-api-pattern
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-pattern-schema.json\",\n  \"title\": \"Pattern\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"problem\": {\n      \"type\": \"string\"\n    },\n    \"solution\": {\n      \"type\": \"string\"\n    },\n    \"consequences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relatedPatterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\
  \n      }\n    },\n    \"applicability\": {\n      \"type\": \"string\"\n    },\n    \"knownUses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-pattern-schema.json
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
title: Pattern
---
