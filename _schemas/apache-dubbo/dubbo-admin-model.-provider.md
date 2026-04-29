---
description: model.Provider schema from Dubbo Admin API
layout: schema
name: model.Provider
properties_list:
- description: ''
  name: address
  type: string
- description: ''
  name: alived
  type: integer
- description: ''
  name: application
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: dynamic
  type: boolean
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: expired
  type: object
- description: ''
  name: hash
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: ids
  type: array
- description: ''
  name: miss
  type: boolean
- description: ''
  name: modified
  type: string
- description: ''
  name: now
  type: string
- description: ''
  name: operator
  type: string
- description: ''
  name: operatorAddress
  type: string
- description: ''
  name: parameters
  type: string
- description: ''
  name: registry
  type: string
- description: ''
  name: registrySource
  type: object
- description: ''
  name: serialization
  type: string
- description: ''
  name: service
  type: string
- description: ''
  name: timeout
  type: integer
- description: ''
  name: url
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: weight
  type: integer
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-provider-schema.json
slug: dubbo-admin-model.-provider
source_filename: dubbo-admin-model.-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-provider-schema.json\",\n  \"title\": \"model.Provider\",\n  \"description\": \"model.Provider schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\"\n    },\n    \"alived\": {\n      \"type\": \"integer\"\n    },\n    \"application\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"dynamic\": {\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"expired\": {\n      \"$ref\": \"#/definitions/time.Duration\"\n    },\n    \"hash\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n    \
  \  }\n    },\n    \"miss\": {\n      \"type\": \"boolean\"\n    },\n    \"modified\": {\n      \"type\": \"string\"\n    },\n    \"now\": {\n      \"type\": \"string\"\n    },\n    \"operator\": {\n      \"type\": \"string\"\n    },\n    \"operatorAddress\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"string\"\n    },\n    \"registry\": {\n      \"type\": \"string\"\n    },\n    \"registrySource\": {\n      \"$ref\": \"#/definitions/model.RegistrySource\"\n    },\n    \"serialization\": {\n      \"type\": \"string\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"weight\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-provider-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Provider
---
