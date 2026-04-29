---
description: model.ConditionRouteDto schema from Dubbo Admin API
layout: schema
name: model.ConditionRouteDto
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: conditions
  type: array
- description: ''
  name: configVersion
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: force
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: runtime
  type: boolean
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
schema_file: json-schema/dubbo-admin-model.-condition-route-dto-schema.json
slug: dubbo-admin-model.-condition-route-dto
source_filename: dubbo-admin-model.-condition-route-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-condition-route-dto-schema.json\",\n  \"title\": \"model.ConditionRouteDto\",\n  \"description\": \"model.ConditionRouteDto schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"configVersion\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"force\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"runtime\": {\n      \"type\": \"boolean\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"serviceGroup\"\
  : {\n      \"type\": \"string\"\n    },\n    \"serviceVersion\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"conditions\",\n    \"configVersion\",\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-condition-route-dto-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ConditionRouteDto
---
