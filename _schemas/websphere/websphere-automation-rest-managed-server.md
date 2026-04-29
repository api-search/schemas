---
description: ''
layout: schema
name: ManagedServer
properties_list:
- description: Unique server identifier
  name: id
  type: string
- description: Server name
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: WebSphere version
  name: version
  type: string
- description: Server hostname
  name: host
  type: string
- description: Server port
  name: port
  type: integer
- description: ''
  name: status
  type: string
- description: Number of open vulnerabilities
  name: vulnerabilityCount
  type: integer
- description: ''
  name: lastScanDate
  type: string
- description: ''
  name: registeredDate
  type: string
- description: List of installed fix IDs
  name: installedFixes
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-managed-server-schema.json
slug: websphere-automation-rest-managed-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedServer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique server identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Server name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"WebSphere version\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Server hostname\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Server port\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"vulnerabilityCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of open vulnerabilities\"\n    },\n    \"lastScanDate\": {\n      \"type\": \"string\"\n    },\n    \"registeredDate\": {\n      \"type\": \"string\"\
  \n    },\n    \"installedFixes\": {\n      \"type\": \"array\",\n      \"description\": \"List of installed fix IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-managed-server-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ManagedServer
---
