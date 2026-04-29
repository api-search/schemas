---
description: CheckpointAlignment schema from Apache Flink REST API
layout: schema
name: CheckpointAlignment
properties_list:
- description: ''
  name: buffered
  type: integer
- description: ''
  name: duration
  type: integer
- description: ''
  name: persisted
  type: integer
- description: ''
  name: processed
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-alignment-schema.json
slug: flink-rest-checkpoint-alignment
source_filename: flink-rest-checkpoint-alignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-alignment-schema.json\",\n  \"title\": \"CheckpointAlignment\",\n  \"description\": \"CheckpointAlignment schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buffered\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"persisted\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"processed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-alignment-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointAlignment
---
