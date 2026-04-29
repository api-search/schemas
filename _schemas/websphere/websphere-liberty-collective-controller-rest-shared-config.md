---
description: ''
layout: schema
name: SharedConfig
properties_list:
- description: Configuration name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Configuration XML content
  name: content
  type: string
- description: ''
  name: lastModified
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-shared-config-schema.json
slug: websphere-liberty-collective-controller-rest-shared-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SharedConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration XML content\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-shared-config-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: SharedConfig
---
