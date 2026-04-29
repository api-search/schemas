---
description: ''
layout: schema
name: ClusterNode
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: hostName
  type: string
- description: ''
  name: grpcPort
  type: integer
- description: ''
  name: httpPort
  type: integer
- description: ''
  name: internalHostName
  type: string
- description: ''
  name: internalGrpcPort
  type: integer
- description: ''
  name: connected
  type: boolean
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-clusternode-schema.json
slug: axon-clusternode
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterNode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"hostName\": {\n      \"type\": \"string\"\n    },\n    \"grpcPort\": {\n      \"type\": \"integer\"\n    },\n    \"httpPort\": {\n      \"type\": \"integer\"\n    },\n    \"internalHostName\": {\n      \"type\": \"string\"\n    },\n    \"internalGrpcPort\": {\n      \"type\": \"integer\"\n    },\n    \"connected\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-clusternode-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: ClusterNode
---
