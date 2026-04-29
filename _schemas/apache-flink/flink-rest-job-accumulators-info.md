---
description: JobAccumulatorsInfo schema from Apache Flink REST API
layout: schema
name: JobAccumulatorsInfo
properties_list:
- description: ''
  name: job-accumulators
  type: array
- description: ''
  name: serialized-user-task-accumulators
  type: object
- description: ''
  name: user-task-accumulators
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-accumulators-info-schema.json
slug: flink-rest-job-accumulators-info
source_filename: flink-rest-job-accumulators-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-accumulators-info-schema.json\",\n  \"title\": \"JobAccumulatorsInfo\",\n  \"description\": \"JobAccumulatorsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job-accumulators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobAccumulator\"\n      }\n    },\n    \"serialized-user-task-accumulators\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/SerializedValueOptionalFailureObject\"\n      }\n    },\n    \"user-task-accumulators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserTaskAccumulator\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-accumulators-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobAccumulatorsInfo
---
