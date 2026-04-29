---
description: ''
layout: schema
name: Channel
properties_list:
- description: Channel name
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: Connection name (host and port)
  name: connectionName
  type: string
- description: Transmission queue name
  name: transmissionQueue
  type: string
- description: ''
  name: status
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-channel-schema.json
slug: websphere-mq-rest-channel
source_filename: websphere-mq-rest-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Channel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Channel name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"connectionName\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name (host and port)\"\n    },\n    \"transmissionQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Transmission queue name\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-channel-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Channel
---
