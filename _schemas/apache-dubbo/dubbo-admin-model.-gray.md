---
description: model.Gray schema from Dubbo Admin API
layout: schema
name: model.Gray
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: tags
  type: array
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-gray-schema.json
slug: dubbo-admin-model.-gray
source_filename: dubbo-admin-model.-gray-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-gray-schema.json\",\n  \"title\": \"model.Gray\",\n  \"description\": \"model.Gray schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.Tag\"\n      }\n    }\n  },\n  \"required\": [\n    \"application\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-gray-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Gray
---
