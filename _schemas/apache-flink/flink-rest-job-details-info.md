---
description: JobDetailsInfo schema from Apache Flink REST API
layout: schema
name: JobDetailsInfo
properties_list:
- description: ''
  name: duration
  type: integer
- description: ''
  name: end-time
  type: integer
- description: ''
  name: isStoppable
  type: boolean
- description: ''
  name: jid
  type: object
- description: ''
  name: job-type
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
  name: pending-operators
  type: integer
- description: ''
  name: plan
  type: object
- description: ''
  name: start-time
  type: integer
- description: ''
  name: state
  type: object
- description: ''
  name: status-counts
  type: object
- description: ''
  name: stream-graph
  type: object
- description: ''
  name: timestamps
  type: object
- description: ''
  name: vertices
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-details-info-schema.json
slug: flink-rest-job-details-info
source_filename: flink-rest-job-details-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-info-schema.json\",\n  \"title\": \"JobDetailsInfo\",\n  \"description\": \"JobDetailsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"isStoppable\": {\n      \"type\": \"boolean\"\n    },\n    \"jid\": {\n      \"$ref\": \"#/components/schemas/JobID\"\n    },\n    \"job-type\": {\n      \"$ref\": \"#/components/schemas/JobType\"\n    },\n    \"maxParallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"now\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n\
  \    \"pending-operators\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"plan\": {\n      \"$ref\": \"#/components/schemas/RawJson\"\n    },\n    \"start-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/JobStatus\"\n    },\n    \"status-counts\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    },\n    \"stream-graph\": {\n      \"$ref\": \"#/components/schemas/RawJson\"\n    },\n    \"timestamps\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    },\n    \"vertices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobDetailsVertexInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobDetailsInfo
---
