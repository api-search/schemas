---
description: JobVertexBackPressureInfo schema from Apache Flink REST API
layout: schema
name: JobVertexBackPressureInfo
properties_list:
- description: ''
  name: backpressureLevel
  type: object
- description: ''
  name: end-timestamp
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: subtasks
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-vertex-back-pressure-info-schema.json
slug: flink-rest-job-vertex-back-pressure-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-back-pressure-info-schema.json\",\n  \"title\": \"JobVertexBackPressureInfo\",\n  \"description\": \"JobVertexBackPressureInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backpressureLevel\": {\n      \"$ref\": \"#/components/schemas/VertexBackPressureLevel\"\n    },\n    \"end-timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/VertexBackPressureStatus\"\n    },\n    \"subtasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskBackPressureInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-back-pressure-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobVertexBackPressureInfo
---
