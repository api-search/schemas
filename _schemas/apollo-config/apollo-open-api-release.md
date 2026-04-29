---
description: Release schema from Apollo Config Open API
layout: schema
name: Release
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: appId
  type: string
- description: ''
  name: clusterName
  type: string
- description: ''
  name: namespaceName
  type: string
- description: Release title
  name: name
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: isAbandoned
  type: boolean
- description: Key-value configuration snapshot at release time
  name: configurations
  type: object
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
schema_file: json-schema/apollo-open-api-release-schema.json
slug: apollo-open-api-release
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-release-schema.json\",\n  \"title\": \"Release\",\n  \"description\": \"Release schema from Apollo Config Open API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\"\n    },\n    \"namespaceName\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Release title\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"isAbandoned\": {\n      \"type\": \"boolean\"\n    },\n    \"configurations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value\
  \ configuration snapshot at release time\"\n    },\n    \"dataChangeCreatedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeLastModifiedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeCreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dataChangeLastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-release-schema.json
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
title: Release
---
