---
description: ''
layout: schema
name: User
properties_list:
- description: ''
  name: userName
  type: string
- description: ''
  name: roles
  type: array
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-user-schema.json
slug: axon-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"context\": {\n            \"type\": \"string\"\n          },\n          \"roles\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-user-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: User
---
