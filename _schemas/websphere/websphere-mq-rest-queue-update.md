---
description: ''
layout: schema
name: QueueUpdate
properties_list:
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
  name: inhibitPut
  type: boolean
- description: ''
  name: inhibitGet
  type: boolean
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-queue-update-schema.json
slug: websphere-mq-rest-queue-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"maxDepth\": {\n      \"type\": \"integer\"\n    },\n    \"maxMessageLength\": {\n      \"type\": \"integer\"\n    },\n    \"inhibitPut\": {\n      \"type\": \"boolean\"\n    },\n    \"inhibitGet\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-queue-update-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: QueueUpdate
---
