---
description: JobVertexTaskManagerInfo schema from Apache Flink REST API
layout: schema
name: JobVertexTaskManagerInfo
properties_list:
- description: ''
  name: aggregated
  type: object
- description: ''
  name: duration
  type: integer
- description: ''
  name: end-time
  type: integer
- description: ''
  name: endpoint
  type: string
- description: ''
  name: metrics
  type: object
- description: ''
  name: start-time
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: status-counts
  type: object
- description: ''
  name: taskmanager-id
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-vertex-task-manager-info-schema.json
slug: flink-rest-job-vertex-task-manager-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-task-manager-info-schema.json\",\n  \"title\": \"JobVertexTaskManagerInfo\",\n  \"description\": \"JobVertexTaskManagerInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregated\": {\n      \"$ref\": \"#/components/schemas/AggregatedTaskDetailsInfo\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/IOMetricsInfo\"\n    },\n    \"start-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ExecutionState\"\n   \
  \ },\n    \"status-counts\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    },\n    \"taskmanager-id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-task-manager-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobVertexTaskManagerInfo
---
