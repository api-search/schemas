---
description: RestoredCheckpointStatistics schema from Apache Flink REST API
layout: schema
name: RestoredCheckpointStatistics
properties_list:
- description: ''
  name: external_path
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: is_savepoint
  type: boolean
- description: ''
  name: restore_timestamp
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-restored-checkpoint-statistics-schema.json
slug: flink-rest-restored-checkpoint-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-restored-checkpoint-statistics-schema.json\",\n  \"title\": \"RestoredCheckpointStatistics\",\n  \"description\": \"RestoredCheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external_path\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"is_savepoint\": {\n      \"type\": \"boolean\"\n    },\n    \"restore_timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-restored-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: RestoredCheckpointStatistics
---
