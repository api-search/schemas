---
description: Item schema from Apollo Config Open API
layout: schema
name: Item
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: namespaceId
  type: integer
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: lineNum
  type: integer
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
schema_file: json-schema/apollo-open-api-item-schema.json
slug: apollo-open-api-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-item-schema.json\",\n  \"title\": \"Item\",\n  \"description\": \"Item schema from Apollo Config Open API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"namespaceId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"lineNum\": {\n      \"type\": \"integer\"\n    },\n    \"dataChangeCreatedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeLastModifiedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeCreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"\
  dataChangeLastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-item-schema.json
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
title: Item
---
