---
description: SubtaskCheckpointStatistics schema from Apache Flink REST API
layout: schema
name: SubtaskCheckpointStatistics
properties_list:
- description: ''
  name: className
  type: string
- description: ''
  name: index
  type: integer
- description: ''
  name: status
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-checkpoint-statistics-schema.json
slug: flink-rest-subtask-checkpoint-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-checkpoint-statistics-schema.json\",\n  \"title\": \"SubtaskCheckpointStatistics\",\n  \"description\": \"SubtaskCheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"className\": {\n      \"type\": \"string\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"className\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskCheckpointStatistics
---
