---
description: SubtaskExecutionAttemptAccumulatorsInfo schema from Apache Flink REST API
layout: schema
name: SubtaskExecutionAttemptAccumulatorsInfo
properties_list:
- description: ''
  name: attempt
  type: integer
- description: ''
  name: id
  type: string
- description: ''
  name: subtask
  type: integer
- description: ''
  name: user-accumulators
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-execution-attempt-accumulators-info-schema.json
slug: flink-rest-subtask-execution-attempt-accumulators-info
source_filename: flink-rest-subtask-execution-attempt-accumulators-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-execution-attempt-accumulators-info-schema.json\",\n  \"title\": \"SubtaskExecutionAttemptAccumulatorsInfo\",\n  \"description\": \"SubtaskExecutionAttemptAccumulatorsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attempt\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"subtask\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"user-accumulators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserAccumulator\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-execution-attempt-accumulators-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskExecutionAttemptAccumulatorsInfo
---
