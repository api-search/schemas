---
description: ''
layout: schema
name: ConfigElement
properties_list:
- description: Unique identifier
  name: uid
  type: string
- description: Configuration element type name
  name: configElementName
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-config-element-schema.json
slug: websphere-liberty-admin-rest-config-element
source_filename: websphere-liberty-admin-rest-config-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigElement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier\"\n    },\n    \"configElementName\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration element type name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-config-element-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ConfigElement
---
