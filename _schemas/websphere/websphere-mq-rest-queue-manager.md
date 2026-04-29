---
description: ''
layout: schema
name: QueueManager
properties_list:
- description: Queue manager name
  name: name
  type: string
- description: Queue manager state
  name: state
  type: string
- description: MQ version
  name: version
  type: string
- description: Platform type
  name: platform
  type: string
- description: Command level
  name: commandLevel
  type: integer
- description: Number of active connections
  name: connectionCount
  type: integer
- description: ''
  name: description
  type: string
- description: Maximum message length in bytes
  name: maximumMessageLength
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-queue-manager-schema.json
slug: websphere-mq-rest-queue-manager
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueManager\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Queue manager name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Queue manager state\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"MQ version\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Platform type\"\n    },\n    \"commandLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Command level\"\n    },\n    \"connectionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active connections\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"maximumMessageLength\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum message length in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-queue-manager-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: QueueManager
---
