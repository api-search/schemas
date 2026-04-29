---
description: SubtaskBackPressureInfo schema from Apache Flink REST API
layout: schema
name: SubtaskBackPressureInfo
properties_list:
- description: ''
  name: attempt-number
  type: integer
- description: ''
  name: backpressureLevel
  type: object
- description: ''
  name: busyRatio
  type: number
- description: ''
  name: idleRatio
  type: number
- description: ''
  name: other-concurrent-attempts
  type: array
- description: ''
  name: ratio
  type: number
- description: ''
  name: subtask
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-back-pressure-info-schema.json
slug: flink-rest-subtask-back-pressure-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-back-pressure-info-schema.json\",\n  \"title\": \"SubtaskBackPressureInfo\",\n  \"description\": \"SubtaskBackPressureInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attempt-number\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"backpressureLevel\": {\n      \"$ref\": \"#/components/schemas/VertexBackPressureLevel\"\n    },\n    \"busyRatio\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"idleRatio\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"other-concurrent-attempts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskBackPressureInfo\"\n      }\n    },\n    \"ratio\": {\n      \"type\": \"number\"\
  ,\n      \"format\": \"double\"\n    },\n    \"subtask\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-back-pressure-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskBackPressureInfo
---
