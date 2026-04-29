---
description: ''
layout: schema
name: CreateContextRequest
properties_list:
- description: ''
  name: context
  type: string
- description: ''
  name: replicationGroup
  type: string
- description: ''
  name: nodes
  type: array
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-createcontextrequest-schema.json
slug: axon-createcontextrequest
source_filename: axon-createcontextrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateContextRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"string\"\n    },\n    \"replicationGroup\": {\n      \"type\": \"string\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n    \"context\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-createcontextrequest-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: CreateContextRequest
---
