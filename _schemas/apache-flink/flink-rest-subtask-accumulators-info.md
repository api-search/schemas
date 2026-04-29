---
description: SubtaskAccumulatorsInfo schema from Apache Flink REST API
layout: schema
name: SubtaskAccumulatorsInfo
properties_list:
- description: ''
  name: attempt
  type: integer
- description: ''
  name: endpoint
  type: string
- description: ''
  name: subtask
  type: integer
- description: ''
  name: user-accumulators
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-accumulators-info-schema.json
slug: flink-rest-subtask-accumulators-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-accumulators-info-schema.json\",\n  \"title\": \"SubtaskAccumulatorsInfo\",\n  \"description\": \"SubtaskAccumulatorsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attempt\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"subtask\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"user-accumulators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserAccumulator\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-accumulators-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskAccumulatorsInfo
---
