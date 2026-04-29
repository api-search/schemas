---
description: ''
layout: schema
name: Queue
properties_list:
- description: Queue name
  name: name
  type: string
- description: Queue type
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: Maximum queue depth
  name: maxDepth
  type: integer
- description: Maximum message length in bytes
  name: maxMessageLength
  type: integer
- description: Current number of messages on the queue
  name: currentDepth
  type: integer
- description: Whether put operations are inhibited
  name: inhibitPut
  type: boolean
- description: Whether get operations are inhibited
  name: inhibitGet
  type: boolean
- description: ''
  name: persistence
  type: object
- description: ''
  name: cluster
  type: object
- description: ''
  name: status
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-queue-schema.json
slug: websphere-mq-rest-queue
source_filename: websphere-mq-rest-queue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Queue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Queue name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Queue type\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"maxDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum queue depth\"\n    },\n    \"maxMessageLength\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum message length in bytes\"\n    },\n    \"currentDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of messages on the queue\"\n    },\n    \"inhibitPut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether put operations are inhibited\"\n    },\n    \"inhibitGet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether get operations are inhibited\"\
  \n    },\n    \"persistence\": {\n      \"type\": \"object\"\n    },\n    \"cluster\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-queue-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Queue
---
