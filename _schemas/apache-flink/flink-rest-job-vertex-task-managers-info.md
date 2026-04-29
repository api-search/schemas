---
description: JobVertexTaskManagersInfo schema from Apache Flink REST API
layout: schema
name: JobVertexTaskManagersInfo
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: now
  type: integer
- description: ''
  name: taskmanagers
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-vertex-task-managers-info-schema.json
slug: flink-rest-job-vertex-task-managers-info
source_filename: flink-rest-job-vertex-task-managers-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-task-managers-info-schema.json\",\n  \"title\": \"JobVertexTaskManagersInfo\",\n  \"description\": \"JobVertexTaskManagersInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"$ref\": \"#/components/schemas/JobVertexID\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"now\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"taskmanagers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobVertexTaskManagerInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-task-managers-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobVertexTaskManagersInfo
---
