---
description: ''
layout: schema
name: DomainList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: domains
  type: array
provider_name: Architecture Pattern
provider_slug: architecture-pattern
schema_file: json-schema/architecture-pattern-api-domain-list-schema.json
slug: architecture-pattern-api-domain-list
source_filename: architecture-pattern-api-domain-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-domain-list-schema.json\",\n  \"title\": \"DomainList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"name\": {},\n          \"description\": {},\n          \"patternCount\": {},\n          \"subdomains\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/json-schema/architecture-pattern-api-domain-list-schema.json
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
title: DomainList
---
