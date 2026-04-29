---
description: Namespace schema from Apollo Config Open API
layout: schema
name: Namespace
properties_list:
- description: ''
  name: appId
  type: string
- description: ''
  name: clusterName
  type: string
- description: ''
  name: namespaceName
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: format
  type: string
- description: ''
  name: isPublic
  type: boolean
- description: ''
  name: items
  type: array
- description: ''
  name: dataChangeCreatedBy
  type: string
- description: ''
  name: dataChangeLastModifiedBy
  type: string
- description: ''
  name: dataChangeCreatedTime
  type: string
- description: ''
  name: dataChangeLastModifiedTime
  type: string
provider_name: Apollo Config
provider_slug: apollo-config
schema_file: json-schema/apollo-open-api-namespace-schema.json
slug: apollo-open-api-namespace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-namespace-schema.json\",\n  \"title\": \"Namespace\",\n  \"description\": \"Namespace schema from Apollo Config Open API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\"\n    },\n    \"namespaceName\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"properties\",\n        \"xml\",\n        \"json\",\n        \"yml\",\n        \"yaml\",\n        \"txt\"\n      ]\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Item\"\n      }\n    },\n    \"\
  dataChangeCreatedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeLastModifiedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeCreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dataChangeLastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-namespace-schema.json
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
title: Namespace
---
