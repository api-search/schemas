---
description: ''
layout: schema
name: LogMessage
properties_list:
- description: ''
  name: datetime
  type: string
- description: ''
  name: level
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: logger
  type: string
- description: ''
  name: thread
  type: string
- description: ''
  name: sequence
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-log-message-schema.json
slug: websphere-liberty-admin-rest-log-message
source_filename: websphere-liberty-admin-rest-log-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogMessage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datetime\": {\n      \"type\": \"string\"\n    },\n    \"level\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"logger\": {\n      \"type\": \"string\"\n    },\n    \"thread\": {\n      \"type\": \"string\"\n    },\n    \"sequence\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-log-message-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: LogMessage
---
