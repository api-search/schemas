---
description: ''
layout: schema
name: ServerHealth
properties_list:
- description: ''
  name: serverId
  type: string
- description: ''
  name: serverName
  type: string
- description: ''
  name: status
  type: string
- description: Uptime in seconds
  name: uptime
  type: integer
- description: CPU usage percentage
  name: cpuUsage
  type: number
- description: Memory usage percentage
  name: memoryUsage
  type: number
- description: ''
  name: openVulnerabilities
  type: integer
- description: ''
  name: lastHealthCheck
  type: string
- description: ''
  name: checks
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-server-health-schema.json
slug: websphere-automation-rest-server-health
source_filename: websphere-automation-rest-server-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerHealth\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverId\": {\n      \"type\": \"string\"\n    },\n    \"serverName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Uptime in seconds\"\n    },\n    \"cpuUsage\": {\n      \"type\": \"number\",\n      \"description\": \"CPU usage percentage\"\n    },\n    \"memoryUsage\": {\n      \"type\": \"number\",\n      \"description\": \"Memory usage percentage\"\n    },\n    \"openVulnerabilities\": {\n      \"type\": \"integer\"\n    },\n    \"lastHealthCheck\": {\n      \"type\": \"string\"\n    },\n    \"checks\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-server-health-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ServerHealth
---
