---
description: ''
layout: schema
name: CreateUserRequest
properties_list:
- description: ''
  name: userName
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: roles
  type: array
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-createuserrequest-schema.json
slug: axon-createuserrequest
source_filename: axon-createuserrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateUserRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"context\": {\n            \"type\": \"string\"\n          },\n          \"roles\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"userName\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-createuserrequest-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: CreateUserRequest
---
