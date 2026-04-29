---
description: Information about local zone partition state.
layout: schema
name: LocalZonePartitionStateResponse
properties_list:
- description: ''
  name: partitionId
  type: integer
- description: ''
  name: zoneName
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
schema_file: json-schema/rest-api-local-zone-partition-state-response-schema.json
slug: rest-api-local-zone-partition-state-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-local-zone-partition-state-response-schema.json\",\n  \"title\": \"LocalZonePartitionStateResponse\",\n  \"description\": \"Information about local zone partition state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partitionId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"zoneName\": {\n      \"type\": \"string\"\n    },\n    \"nodeName\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"estimatedRows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"estimatedRows\",\n    \"nodeName\",\n    \"partitionId\",\n    \"state\",\n    \"zoneName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-local-zone-partition-state-response-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: LocalZonePartitionStateResponse
---
