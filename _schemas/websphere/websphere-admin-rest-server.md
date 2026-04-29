---
description: ''
layout: schema
name: Server
properties_list:
- description: Server name
  name: name
  type: string
- description: Node where the server resides
  name: nodeName
  type: string
- description: Cluster membership
  name: clusterName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: serverType
  type: string
- description: Process ID
  name: pid
  type: integer
- description: ''
  name: ports
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-server-schema.json
slug: websphere-admin-rest-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Server name\"\n    },\n    \"nodeName\": {\n      \"type\": \"string\",\n      \"description\": \"Node where the server resides\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster membership\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"serverType\": {\n      \"type\": \"string\"\n    },\n    \"pid\": {\n      \"type\": \"integer\",\n      \"description\": \"Process ID\"\n    },\n    \"ports\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-server-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Server
---
