---
description: model.ServiceDTO schema from Dubbo Admin API
layout: schema
name: model.ServiceDTO
properties_list:
- description: ''
  name: appName
  type: string
- description: ''
  name: group
  type: string
- description: ''
  name: registrySource
  type: object
- description: ''
  name: service
  type: string
- description: ''
  name: version
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-service-dto-schema.json
slug: dubbo-admin-model.-service-dto
source_filename: dubbo-admin-model.-service-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-service-dto-schema.json\",\n  \"title\": \"model.ServiceDTO\",\n  \"description\": \"model.ServiceDTO schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appName\": {\n      \"type\": \"string\"\n    },\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"registrySource\": {\n      \"$ref\": \"#/definitions/model.RegistrySource\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-service-dto-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ServiceDTO
---
