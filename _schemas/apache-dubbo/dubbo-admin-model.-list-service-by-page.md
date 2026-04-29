---
description: model.ListServiceByPage schema from Dubbo Admin API
layout: schema
name: model.ListServiceByPage
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: first
  type: boolean
- description: ''
  name: last
  type: boolean
- description: ''
  name: offset
  type: integer
- description: ''
  name: pageNumber
  type: string
- description: ''
  name: size
  type: string
- description: ''
  name: totalElements
  type: integer
- description: ''
  name: totalPages
  type: integer
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-list-service-by-page-schema.json
slug: dubbo-admin-model.-list-service-by-page
source_filename: dubbo-admin-model.-list-service-by-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-list-service-by-page-schema.json\",\n  \"title\": \"model.ListServiceByPage\",\n  \"description\": \"model.ListServiceByPage schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.ServiceDTO\"\n      }\n    },\n    \"first\": {\n      \"type\": \"boolean\"\n    },\n    \"last\": {\n      \"type\": \"boolean\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"string\"\n    },\n    \"totalElements\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-list-service-by-page-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ListServiceByPage
---
