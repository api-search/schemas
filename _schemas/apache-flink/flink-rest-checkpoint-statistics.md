---
description: CheckpointStatistics schema from Apache Flink REST API
layout: schema
name: CheckpointStatistics
properties_list:
- description: ''
  name: alignment_buffered
  type: integer
- description: ''
  name: checkpoint_type
  type: object
- description: ''
  name: checkpointed_size
  type: integer
- description: ''
  name: className
  type: string
- description: ''
  name: end_to_end_duration
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: is_savepoint
  type: boolean
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
  name: savepointFormat
  type: string
- description: ''
  name: state_size
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: tasks
  type: object
- description: ''
  name: trigger_timestamp
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-statistics-schema.json
slug: flink-rest-checkpoint-statistics
source_filename: flink-rest-checkpoint-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-statistics-schema.json\",\n  \"title\": \"CheckpointStatistics\",\n  \"description\": \"CheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alignment_buffered\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"checkpoint_type\": {\n      \"$ref\": \"#/components/schemas/RestAPICheckpointType\"\n    },\n    \"checkpointed_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"className\": {\n      \"type\": \"string\"\n    },\n    \"end_to_end_duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"is_savepoint\": {\n      \"type\": \"boolean\"\n    },\n    \"\
  latest_ack_timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"num_acknowledged_subtasks\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"num_subtasks\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"persisted_data\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"processed_data\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"savepointFormat\": {\n      \"type\": \"string\"\n    },\n    \"state_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/CheckpointStatsStatus\"\n    },\n    \"tasks\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/TaskCheckpointStatistics\"\n      }\n    },\n    \"trigger_timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\"\
  : [\n    \"className\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointStatistics
---
