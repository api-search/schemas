---
description: model.DynamicConfig schema from Dubbo Admin API
layout: schema
name: model.DynamicConfig
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: configVersion
  type: string
- description: ''
  name: configs
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: service
  type: string
- description: ''
  name: serviceGroup
  type: string
- description: ''
  name: serviceVersion
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-dynamic-config-schema.json
slug: dubbo-admin-model.-dynamic-config
source_filename: dubbo-admin-model.-dynamic-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-dynamic-config-schema.json\",\n  \"title\": \"model.DynamicConfig\",\n  \"description\": \"model.DynamicConfig schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\"\n    },\n    \"configVersion\": {\n      \"type\": \"string\"\n    },\n    \"configs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.OverrideConfig\"\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"serviceGroup\": {\n      \"type\": \"string\"\n    },\n    \"serviceVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-dynamic-config-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.DynamicConfig
---
