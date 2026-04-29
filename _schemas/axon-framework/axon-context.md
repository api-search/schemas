---
description: ''
layout: schema
name: Context
properties_list:
- description: ''
  name: context
  type: string
- description: ''
  name: leader
  type: string
- description: ''
  name: roles
  type: array
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-context-schema.json
slug: axon-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Context\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"string\"\n    },\n    \"leader\": {\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"node\": {\n            \"type\": \"string\"\n          },\n          \"role\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-context-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: Context
---
