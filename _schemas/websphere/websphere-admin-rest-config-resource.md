---
description: ''
layout: schema
name: ConfigResource
properties_list:
- description: Resource identifier
  name: id
  type: string
- description: Resource type
  name: type
  type: string
- description: Resource display name
  name: name
  type: string
- description: Resource attributes
  name: attributes
  type: object
- description: ''
  name: links
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-config-resource-schema.json
slug: websphere-admin-rest-config-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource display name\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Resource attributes\"\n    },\n    \"links\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-config-resource-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ConfigResource
---
