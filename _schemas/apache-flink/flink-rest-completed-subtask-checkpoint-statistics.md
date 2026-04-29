---
description: CompletedSubtaskCheckpointStatistics schema from Apache Flink REST API
layout: schema
name: CompletedSubtaskCheckpointStatistics
properties_list: []
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-completed-subtask-checkpoint-statistics-schema.json
slug: flink-rest-completed-subtask-checkpoint-statistics
source_filename: flink-rest-completed-subtask-checkpoint-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-completed-subtask-checkpoint-statistics-schema.json\",\n  \"title\": \"CompletedSubtaskCheckpointStatistics\",\n  \"description\": \"CompletedSubtaskCheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/SubtaskCheckpointStatistics\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ack_timestamp\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"end_to_end_duration\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"checkpointed_size\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"state_size\": {\n          \"type\": \"integer\",\n          \"\
  format\": \"int64\"\n        },\n        \"checkpoint\": {\n          \"$ref\": \"#/components/schemas/CheckpointDuration\"\n        },\n        \"alignment\": {\n          \"$ref\": \"#/components/schemas/CheckpointAlignment\"\n        },\n        \"start_delay\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"unaligned_checkpoint\": {\n          \"type\": \"boolean\"\n        },\n        \"aborted\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-completed-subtask-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CompletedSubtaskCheckpointStatistics
---
