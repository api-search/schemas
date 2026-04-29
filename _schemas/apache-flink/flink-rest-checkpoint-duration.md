---
description: CheckpointDuration schema from Apache Flink REST API
layout: schema
name: CheckpointDuration
properties_list:
- description: ''
  name: async
  type: integer
- description: ''
  name: sync
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-duration-schema.json
slug: flink-rest-checkpoint-duration
source_filename: flink-rest-checkpoint-duration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-duration-schema.json\",\n  \"title\": \"CheckpointDuration\",\n  \"description\": \"CheckpointDuration schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"async\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"sync\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-duration-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointDuration
---
