---
description: Cluster schema from Apollo Config Open API
layout: schema
name: Cluster
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: appId
  type: string
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
schema_file: json-schema/apollo-open-api-cluster-schema.json
slug: apollo-open-api-cluster
source_filename: apollo-open-api-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"Cluster schema from Apollo Config Open API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeCreatedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeLastModifiedBy\": {\n      \"type\": \"string\"\n    },\n    \"dataChangeCreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dataChangeLastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/json-schema/apollo-open-api-cluster-schema.json
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
title: Cluster
---
