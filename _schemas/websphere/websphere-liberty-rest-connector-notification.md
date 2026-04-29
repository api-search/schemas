---
description: ''
layout: schema
name: Notification
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: sequenceNumber
  type: integer
- description: ''
  name: timestamp
  type: integer
- description: ''
  name: userData
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-rest-connector-notification-schema.json
slug: websphere-liberty-rest-connector-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Notification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"sequenceNumber\": {\n      \"type\": \"integer\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\"\n    },\n    \"userData\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-rest-connector-notification-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Notification
---
