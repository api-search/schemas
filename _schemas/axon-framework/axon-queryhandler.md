---
description: ''
layout: schema
name: QueryHandler
properties_list:
- description: ''
  name: query
  type: string
- description: ''
  name: clientId
  type: string
- description: ''
  name: componentName
  type: string
- description: ''
  name: resultName
  type: string
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-queryhandler-schema.json
slug: axon-queryhandler
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryHandler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\"\n    },\n    \"clientId\": {\n      \"type\": \"string\"\n    },\n    \"componentName\": {\n      \"type\": \"string\"\n    },\n    \"resultName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-queryhandler-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: QueryHandler
---
