---
description: An Allianz technology standard definition
layout: schema
name: Standard
properties_list:
- description: Unique identifier for the standard
  name: standard_id
  type: string
- description: Human-readable name of the standard
  name: name
  type: string
- description: Category of the technology standard
  name: category
  type: string
- description: Current version of the standard
  name: version
  type: string
- description: Lifecycle status of the standard
  name: status
  type: string
- description: Description of what the standard covers
  name: description
  type: string
- description: List of rules defined by this standard
  name: rules
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-standard-schema.json
slug: tech-standards-standard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-schema.json\",\n  \"title\": \"Standard\",\n  \"description\": \"An Allianz technology standard definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"standard_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the standard\",\n      \"example\": \"std-500001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the standard\",\n      \"example\": \"REST API Pagination Standard\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the technology standard\",\n      \"enum\": [\n        \"api-design\",\n        \"backend\",\n        \"architecture\",\n        \"security\",\n        \"testing\"\n      ],\n      \"example\": \"api-design\"\
  \n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current version of the standard\",\n      \"example\": \"2.1.0\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle status of the standard\",\n      \"enum\": [\n        \"draft\",\n        \"current\",\n        \"deprecated\",\n        \"retired\"\n      ],\n      \"example\": \"current\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the standard covers\",\n      \"example\": \"Standard for paginating collection responses in Allianz REST APIs\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"List of rules defined by this standard\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StandardRule\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: Standard
---
