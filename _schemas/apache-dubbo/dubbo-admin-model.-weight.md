---
description: model.Weight schema from Dubbo Admin API
layout: schema
name: model.Weight
properties_list:
- description: ''
  name: match
  type: object
- description: ''
  name: weight
  type: integer
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-weight-schema.json
slug: dubbo-admin-model.-weight
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-weight-schema.json\",\n  \"title\": \"model.Weight\",\n  \"description\": \"model.Weight schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"match\": {\n      \"$ref\": \"#/definitions/model.ConditionMatch\"\n    },\n    \"weight\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"match\",\n    \"weight\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-weight-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.Weight
---
