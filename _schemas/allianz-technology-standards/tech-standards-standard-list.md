---
description: Paginated list of technology standards
layout: schema
name: StandardList
properties_list:
- description: Total number of standards
  name: total
  type: integer
- description: List of standard records
  name: items
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-standard-list-schema.json
slug: tech-standards-standard-list
source_filename: tech-standards-standard-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-list-schema.json\",\n  \"title\": \"StandardList\",\n  \"description\": \"Paginated list of technology standards\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of standards\",\n      \"example\": 12\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of standard records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Standard\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-list-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: StandardList
---
