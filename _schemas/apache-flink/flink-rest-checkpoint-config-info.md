---
description: CheckpointConfigInfo schema from Apache Flink REST API
layout: schema
name: CheckpointConfigInfo
properties_list:
- description: ''
  name: aligned_checkpoint_timeout
  type: integer
- description: ''
  name: changelog_periodic_materialization_interval
  type: integer
- description: ''
  name: changelog_storage
  type: string
- description: ''
  name: checkpoint_storage
  type: string
- description: ''
  name: checkpoints_after_tasks_finish
  type: boolean
- description: ''
  name: externalization
  type: object
- description: ''
  name: interval
  type: integer
- description: ''
  name: max_concurrent
  type: integer
- description: ''
  name: min_pause
  type: integer
- description: ''
  name: mode
  type: object
- description: ''
  name: state_backend
  type: string
- description: ''
  name: state_changelog_enabled
  type: boolean
- description: ''
  name: timeout
  type: integer
- description: ''
  name: tolerable_failed_checkpoints
  type: integer
- description: ''
  name: unaligned_checkpoints
  type: boolean
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-config-info-schema.json
slug: flink-rest-checkpoint-config-info
source_filename: flink-rest-checkpoint-config-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-config-info-schema.json\",\n  \"title\": \"CheckpointConfigInfo\",\n  \"description\": \"CheckpointConfigInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aligned_checkpoint_timeout\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"changelog_periodic_materialization_interval\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"changelog_storage\": {\n      \"type\": \"string\"\n    },\n    \"checkpoint_storage\": {\n      \"type\": \"string\"\n    },\n    \"checkpoints_after_tasks_finish\": {\n      \"type\": \"boolean\"\n    },\n    \"externalization\": {\n      \"$ref\": \"#/components/schemas/ExternalizedCheckpointInfo\"\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n \
  \     \"format\": \"int64\"\n    },\n    \"max_concurrent\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"min_pause\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"mode\": {\n      \"$ref\": \"#/components/schemas/ProcessingMode\"\n    },\n    \"state_backend\": {\n      \"type\": \"string\"\n    },\n    \"state_changelog_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"tolerable_failed_checkpoints\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"unaligned_checkpoints\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-config-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointConfigInfo
---
