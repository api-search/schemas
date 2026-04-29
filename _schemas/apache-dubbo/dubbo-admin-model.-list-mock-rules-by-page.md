---
description: model.ListMockRulesByPage schema from Dubbo Admin API
layout: schema
name: model.ListMockRulesByPage
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache Dubbo
provider_slug: apache-dubbo
schema_file: json-schema/dubbo-admin-model.-list-mock-rules-by-page-schema.json
slug: dubbo-admin-model.-list-mock-rules-by-page
source_filename: dubbo-admin-model.-list-mock-rules-by-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-list-mock-rules-by-page-schema.json\",\n  \"title\": \"model.ListMockRulesByPage\",\n  \"description\": \"model.ListMockRulesByPage schema from Dubbo Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/model.MockRule\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dubbo/refs/heads/main/json-schema/dubbo-admin-model.-list-mock-rules-by-page-schema.json
tags:
- Apache
- Go
- Java
- Microservices
- Open Source
- RPC
- Service Discovery
- Service Mesh
title: model.ListMockRulesByPage
---
