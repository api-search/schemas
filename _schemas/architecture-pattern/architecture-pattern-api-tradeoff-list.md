---
description: ''
layout: schema
name: TradeoffList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: tradeoffs
  type: array
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-tradeoff-list-schema.json
slug: architecture-pattern-api-tradeoff-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-tradeoff-list-schema.json\",\n  \"title\": \"TradeoffList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"tradeoffs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"patternId\": {},\n          \"dimension\": {},\n          \"benefit\": {},\n          \"drawback\": {},\n          \"severity\": {},\n          \"notes\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-tradeoff-list-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: TradeoffList
---
