---
description: ''
layout: schema
name: User
properties_list:
- description: ''
  name: uid
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: groups
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-user-schema.json
slug: websphere-admin-rest-user
source_filename: websphere-admin-rest-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"groups\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-user-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: User
---
