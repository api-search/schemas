---
description: CheckpointInfo schema from Apache Flink REST API
layout: schema
name: CheckpointInfo
properties_list:
- description: ''
  name: checkpointId
  type: integer
- description: ''
  name: failureCause
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-info-schema.json
slug: flink-rest-checkpoint-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-info-schema.json\",\n  \"title\": \"CheckpointInfo\",\n  \"description\": \"CheckpointInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkpointId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"failureCause\": {\n      \"$ref\": \"#/components/schemas/SerializedThrowable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointInfo
---
