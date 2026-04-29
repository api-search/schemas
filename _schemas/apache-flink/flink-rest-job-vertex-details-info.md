---
description: JobVertexDetailsInfo schema from Apache Flink REST API
layout: schema
name: JobVertexDetailsInfo
properties_list:
- description: ''
  name: aggregated
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: maxParallelism
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: now
  type: integer
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: subtasks
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-vertex-details-info-schema.json
slug: flink-rest-job-vertex-details-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-details-info-schema.json\",\n  \"title\": \"JobVertexDetailsInfo\",\n  \"description\": \"JobVertexDetailsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregated\": {\n      \"$ref\": \"#/components/schemas/AggregatedTaskDetailsInfo\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/JobVertexID\"\n    },\n    \"maxParallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"now\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"subtasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskExecutionAttemptDetailsInfo\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-vertex-details-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobVertexDetailsInfo
---
