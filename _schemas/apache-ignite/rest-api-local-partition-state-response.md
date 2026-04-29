---
description: Information about local partition state.
layout: schema
name: LocalPartitionStateResponse
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
  name: nodeName
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: estimatedRows
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-local-partition-state-response-schema.json
slug: rest-api-local-partition-state-response
source_filename: rest-api-local-partition-state-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-local-partition-state-response-schema.json\",\n  \"title\": \"LocalPartitionStateResponse\",\n  \"description\": \"Information about local partition state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partitionId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"zoneName\": {\n      \"type\": \"string\"\n    },\n    \"tableId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"schemaName\": {\n      \"type\": \"string\"\n    },\n    \"tableName\": {\n      \"type\": \"string\"\n    },\n    \"nodeName\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"estimatedRows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"estimatedRows\"\
  ,\n    \"nodeName\",\n    \"partitionId\",\n    \"schemaName\",\n    \"state\",\n    \"tableId\",\n    \"tableName\",\n    \"zoneName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-local-partition-state-response-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: LocalPartitionStateResponse
---
