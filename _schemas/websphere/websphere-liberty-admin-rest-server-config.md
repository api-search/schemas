---
description: ''
layout: schema
name: ServerConfig
properties_list:
- description: Server description
  name: description
  type: string
- description: ''
  name: featureManager
  type: object
- description: ''
  name: httpEndpoint
  type: array
- description: ''
  name: application
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-server-config-schema.json
slug: websphere-liberty-admin-rest-server-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServerConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Server description\"\n    },\n    \"featureManager\": {\n      \"type\": \"object\"\n    },\n    \"httpEndpoint\": {\n      \"type\": \"array\"\n    },\n    \"application\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-server-config-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ServerConfig
---
