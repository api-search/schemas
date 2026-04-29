---
description: ''
layout: schema
name: AntiPatternList
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
  name: antiPatterns
  type: array
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
schema_file: json-schema/architectural-design-patterns-api-anti-pattern-list-schema.json
slug: architectural-design-patterns-api-anti-pattern-list
source_filename: architectural-design-patterns-api-anti-pattern-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-anti-pattern-list-schema.json\",\n  \"title\": \"AntiPatternList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"antiPatterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"description\": {},\n          \"symptoms\": {},\n          \"causes\": {},\n          \"refactoredSolution\": {},\n          \"relatedPatterns\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-anti-pattern-list-schema.json
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
title: AntiPatternList
---
