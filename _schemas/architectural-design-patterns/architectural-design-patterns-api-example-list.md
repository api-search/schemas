---
description: ''
layout: schema
name: ExampleList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: examples
  type: array
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
schema_file: json-schema/architectural-design-patterns-api-example-list-schema.json
slug: architectural-design-patterns-api-example-list
source_filename: architectural-design-patterns-api-example-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-example-list-schema.json\",\n  \"title\": \"ExampleList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"examples\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"patternId\": {},\n          \"language\": {},\n          \"title\": {},\n          \"description\": {},\n          \"code\": {},\n          \"notes\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/json-schema/architectural-design-patterns-api-example-list-schema.json
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
title: ExampleList
---
