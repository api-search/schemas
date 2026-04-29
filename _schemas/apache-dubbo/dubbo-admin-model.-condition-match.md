---
description: model.ConditionMatch schema from Dubbo Admin API
layout: schema
name: model.ConditionMatch
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: application
  type: object
- description: ''
  name: param
  type: array
- description: ''
  name: service
  type: object
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-condition-match-schema.json
slug: dubbo-admin-model.-condition-match
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-condition-match-schema.json\",\n  \"title\": \"model.ConditionMatch\",\n  \"description\": \"model.ConditionMatch schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"$ref\": \"#/definitions/model.AddressMatch\"\n    },\n    \"application\": {\n      \"$ref\": \"#/definitions/model.ListStringMatch\"\n    },\n    \"param\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.ParamMatch\"\n      }\n    },\n    \"service\": {\n      \"$ref\": \"#/definitions/model.ListStringMatch\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-condition-match-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ConditionMatch
---
