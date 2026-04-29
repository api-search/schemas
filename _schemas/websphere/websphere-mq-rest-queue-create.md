---
description: ''
layout: schema
name: QueueCreate
properties_list:
- description: Queue name
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: maxDepth
  type: integer
- description: ''
  name: maxMessageLength
  type: integer
- description: ''
  name: persistence
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-queue-create-schema.json
slug: websphere-mq-rest-queue-create
source_filename: websphere-mq-rest-queue-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Queue name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"maxDepth\": {\n      \"type\": \"integer\"\n    },\n    \"maxMessageLength\": {\n      \"type\": \"integer\"\n    },\n    \"persistence\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-queue-create-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: QueueCreate
---
