---
description: TaskCheckpointStatistics schema from Apache Flink REST API
layout: schema
name: TaskCheckpointStatistics
properties_list:
- description: ''
  name: alignment_buffered
  type: integer
- description: ''
  name: checkpointed_size
  type: integer
- description: ''
  name: end_to_end_duration
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: latest_ack_timestamp
  type: integer
- description: ''
  name: num_acknowledged_subtasks
  type: integer
- description: ''
  name: num_subtasks
  type: integer
- description: ''
  name: persisted_data
  type: integer
- description: ''
  name: processed_data
  type: integer
- description: ''
  name: state_size
  type: integer
- description: ''
  name: status
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-checkpoint-statistics-schema.json
slug: flink-rest-task-checkpoint-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-checkpoint-statistics-schema.json\",\n  \"title\": \"TaskCheckpointStatistics\",\n  \"description\": \"TaskCheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alignment_buffered\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"checkpointed_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end_to_end_duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"latest_ack_timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"num_acknowledged_subtasks\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"\
  num_subtasks\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"persisted_data\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"processed_data\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"state_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/CheckpointStatsStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskCheckpointStatistics
---
