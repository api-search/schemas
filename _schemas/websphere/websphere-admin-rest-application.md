---
description: ''
layout: schema
name: Application
properties_list:
- description: Application name
  name: name
  type: string
- description: Current application status
  name: status
  type: string
- description: Context root for web modules
  name: contextRoot
  type: string
- description: Target server or cluster
  name: targetServer
  type: string
- description: ''
  name: deployedModules
  type: array
- description: Last modification timestamp
  name: lastModified
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-application-schema.json
slug: websphere-admin-rest-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current application status\"\n    },\n    \"contextRoot\": {\n      \"type\": \"string\",\n      \"description\": \"Context root for web modules\"\n    },\n    \"targetServer\": {\n      \"type\": \"string\",\n      \"description\": \"Target server or cluster\"\n    },\n    \"deployedModules\": {\n      \"type\": \"array\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-application-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Application
---
