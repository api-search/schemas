---
description: ViolationResponseType schema
layout: schema
name: ViolationResponseType
properties_list:
- description: ''
  name: closed_at
  type: integer
- description: ''
  name: condition_name
  type: string
- description: ''
  name: duration
  type: integer
- description: ''
  name: entity
  type: object
- description: ''
  name: id
  type: integer
- description: ''
  name: label
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: opened_at
  type: integer
- description: ''
  name: policy_name
  type: string
- description: ''
  name: priority
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-violation-response-type-schema.json
slug: openapi-violation-response-type
source_filename: openapi-violation-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-violation-response-type-schema.json\",\n  \"title\": \"ViolationResponseType\",\n  \"description\": \"ViolationResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"closed_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"condition_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"entity\": {\n      \"$ref\": \"#/components/schemas/ViolationEntityResponse\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/ViolationLinksResponse\"\n    },\n    \"\
  opened_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-violation-response-type-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: ViolationResponseType
---
