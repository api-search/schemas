---
description: model.Timeout schema from Dubbo Admin API
layout: schema
name: model.Timeout
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: service
  type: string
- description: ''
  name: timeout
  type: integer
- description: ''
  name: version
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-timeout-schema.json
slug: dubbo-admin-model.-timeout
source_filename: dubbo-admin-model.-timeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-timeout-schema.json\",\n  \"title\": \"model.Timeout\",\n  \"description\": \"model.Timeout schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"service\",\n    \"timeout\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-timeout-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Timeout
---
