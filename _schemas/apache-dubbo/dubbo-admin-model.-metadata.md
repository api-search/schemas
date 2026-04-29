---
description: model.Metadata schema from Dubbo Admin API
layout: schema
name: model.Metadata
properties_list:
- description: ''
  name: configCenter
  type: string
- description: ''
  name: metadataCenter
  type: string
- description: ''
  name: protocols
  type: array
- description: ''
  name: registry
  type: string
- description: ''
  name: rules
  type: array
- description: ''
  name: versions
  type: array
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-metadata-schema.json
slug: dubbo-admin-model.-metadata
source_filename: dubbo-admin-model.-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-metadata-schema.json\",\n  \"title\": \"model.Metadata\",\n  \"description\": \"model.Metadata schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configCenter\": {\n      \"type\": \"string\"\n    },\n    \"metadataCenter\": {\n      \"type\": \"string\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"registry\": {\n      \"type\": \"string\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {}\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-metadata-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Metadata
---
