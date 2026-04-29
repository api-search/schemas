---
description: model.Retry schema from Dubbo Admin API
layout: schema
name: model.Retry
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: retry
  type: integer
- description: ''
  name: service
  type: string
- description: ''
  name: version
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-retry-schema.json
slug: dubbo-admin-model.-retry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-retry-schema.json\",\n  \"title\": \"model.Retry\",\n  \"description\": \"model.Retry schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"retry\": {\n      \"type\": \"integer\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"retry\",\n    \"service\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-retry-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Retry
---
