---
description: ''
layout: schema
name: Notification
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: read
  type: boolean
- description: ''
  name: createdDate
  type: string
- description: ''
  name: relatedResourceId
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-notification-schema.json
slug: websphere-automation-rest-notification
source_filename: websphere-automation-rest-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Notification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"severity\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"read\": {\n      \"type\": \"boolean\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"relatedResourceId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-notification-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Notification
---
