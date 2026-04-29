---
description: ''
layout: schema
name: SecurityRole
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: users
  type: array
- description: ''
  name: groups
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-security-role-schema.json
slug: websphere-admin-rest-security-role
source_filename: websphere-admin-rest-security-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRole\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"users\": {\n      \"type\": \"array\"\n    },\n    \"groups\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-security-role-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: SecurityRole
---
