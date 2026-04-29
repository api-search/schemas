---
description: model.ServiceDetailDTO schema from Dubbo Admin API
layout: schema
name: model.ServiceDetailDTO
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: consumers
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: providers
  type: array
- description: ''
  name: service
  type: string
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-service-detail-dto-schema.json
slug: dubbo-admin-model.-service-detail-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-service-detail-dto-schema.json\",\n  \"title\": \"model.ServiceDetailDTO\",\n  \"description\": \"model.ServiceDetailDTO schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\"\n    },\n    \"consumers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.Consumer\"\n      }\n    },\n    \"metadata\": {},\n    \"providers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.Provider\"\n      }\n    },\n    \"service\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-service-detail-dto-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ServiceDetailDTO
---
