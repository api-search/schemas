---
description: model.OverrideConfig schema from Dubbo Admin API
layout: schema
name: model.OverrideConfig
properties_list:
- description: ''
  name: addresses
  type: array
- description: ''
  name: applications
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: match
  type: object
- description: ''
  name: parameters
  type: object
- description: ''
  name: providerAddresses
  type: array
- description: ''
  name: services
  type: array
- description: ''
  name: side
  type: string
- description: ''
  name: type
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-override-config-schema.json
slug: dubbo-admin-model.-override-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-override-config-schema.json\",\n  \"title\": \"model.OverrideConfig\",\n  \"description\": \"model.OverrideConfig schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"match\": {\n      \"$ref\": \"#/definitions/model.ConditionMatch\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    },\n    \"providerAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"\
  services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"side\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-override-config-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.OverrideConfig
---
