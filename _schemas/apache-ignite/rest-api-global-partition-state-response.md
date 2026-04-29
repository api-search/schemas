---
description: Information about global partition state.
layout: schema
name: GlobalPartitionStateResponse
properties_list:
- description: ''
  name: partitionId
  type: integer
- description: ''
  name: zoneName
  type: string
- description: ''
  name: tableId
  type: integer
- description: ''
  name: schemaName
  type: string
- description: ''
  name: tableName
  type: string
- description: ''
  name: state
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-global-partition-state-response-schema.json
slug: rest-api-global-partition-state-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-global-partition-state-response-schema.json\",\n  \"title\": \"GlobalPartitionStateResponse\",\n  \"description\": \"Information about global partition state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partitionId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"zoneName\": {\n      \"type\": \"string\"\n    },\n    \"tableId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"schemaName\": {\n      \"type\": \"string\"\n    },\n    \"tableName\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"partitionId\",\n    \"schemaName\",\n    \"state\",\n    \"tableId\",\n    \"tableName\",\n    \"zoneName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-global-partition-state-response-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: GlobalPartitionStateResponse
---
