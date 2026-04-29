---
description: model.Tag schema from Dubbo Admin API
layout: schema
name: model.Tag
properties_list:
- description: ''
  name: addresses
  type: array
- description: ''
  name: match
  type: array
- description: ''
  name: name
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-tag-schema.json
slug: dubbo-admin-model.-tag
source_filename: dubbo-admin-model.-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-tag-schema.json\",\n  \"title\": \"model.Tag\",\n  \"description\": \"model.Tag schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"match\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.ParamMatch\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"match\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-tag-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Tag
---
