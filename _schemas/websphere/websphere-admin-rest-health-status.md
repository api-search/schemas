---
description: ''
layout: schema
name: HealthStatus
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: serverName
  type: string
- description: Server uptime in milliseconds
  name: uptime
  type: integer
- description: ''
  name: checks
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-health-status-schema.json
slug: websphere-admin-rest-health-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HealthStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"serverName\": {\n      \"type\": \"string\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Server uptime in milliseconds\"\n    },\n    \"checks\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-health-status-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: HealthStatus
---
