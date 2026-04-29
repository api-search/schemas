---
description: SubtaskExecutionAttemptDetailsInfo schema from Apache Flink REST API
layout: schema
name: SubtaskExecutionAttemptDetailsInfo
properties_list:
- description: ''
  name: attempt
  type: integer
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
  name: other-concurrent-attempts
  type: array
- description: ''
  name: start-time
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: status-duration
  type: object
- description: ''
  name: subtask
  type: integer
- description: ''
  name: taskmanager-id
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-execution-attempt-details-info-schema.json
slug: flink-rest-subtask-execution-attempt-details-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-execution-attempt-details-info-schema.json\",\n  \"title\": \"SubtaskExecutionAttemptDetailsInfo\",\n  \"description\": \"SubtaskExecutionAttemptDetailsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attempt\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/IOMetricsInfo\"\n    },\n    \"other-concurrent-attempts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskExecutionAttemptDetailsInfo\"\
  \n      }\n    },\n    \"start-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ExecutionState\"\n    },\n    \"status-duration\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    },\n    \"subtask\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"taskmanager-id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-execution-attempt-details-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskExecutionAttemptDetailsInfo
---
