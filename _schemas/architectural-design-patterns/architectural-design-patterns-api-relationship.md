---
description: ''
layout: schema
name: Relationship
properties_list:
- description: ''
  name: sourcePatternId
  type: string
- description: ''
  name: targetPatternId
  type: string
- description: ''
  name: relationshipType
  type: string
- description: ''
  name: description
  type: string
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
schema_file: json-schema/architectural-design-patterns-api-relationship-schema.json
slug: architectural-design-patterns-api-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-relationship-schema.json\",\n  \"title\": \"Relationship\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourcePatternId\": {\n      \"type\": \"string\"\n    },\n    \"targetPatternId\": {\n      \"type\": \"string\"\n    },\n    \"relationshipType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"uses\",\n        \"extends\",\n        \"alternative\",\n        \"related\",\n        \"conflicts\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-relationship-schema.json
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
title: Relationship
---
