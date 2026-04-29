---
description: JobDetailsVertexInfo schema from Apache Flink REST API
layout: schema
name: JobDetailsVertexInfo
properties_list:
- description: ''
  name: duration
  type: integer
- description: ''
  name: end-time
  type: integer
- description: ''
  name: id
  type: object
- description: ''
  name: maxParallelism
  type: integer
- description: ''
  name: metrics
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: slotSharingGroupId
  type: object
- description: ''
  name: start-time
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: tasks
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-details-vertex-info-schema.json
slug: flink-rest-job-details-vertex-info
source_filename: flink-rest-job-details-vertex-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-vertex-info-schema.json\",\n  \"title\": \"JobDetailsVertexInfo\",\n  \"description\": \"JobDetailsVertexInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/JobVertexID\"\n    },\n    \"maxParallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/IOMetricsInfo\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"slotSharingGroupId\"\
  : {\n      \"$ref\": \"#/components/schemas/SlotSharingGroupId\"\n    },\n    \"start-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ExecutionState\"\n    },\n    \"tasks\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-vertex-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobDetailsVertexInfo
---
