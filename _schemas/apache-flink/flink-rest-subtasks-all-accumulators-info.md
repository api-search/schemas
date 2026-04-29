---
description: SubtasksAllAccumulatorsInfo schema from Apache Flink REST API
layout: schema
name: SubtasksAllAccumulatorsInfo
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: subtasks
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtasks-all-accumulators-info-schema.json
slug: flink-rest-subtasks-all-accumulators-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtasks-all-accumulators-info-schema.json\",\n  \"title\": \"SubtasksAllAccumulatorsInfo\",\n  \"description\": \"SubtasksAllAccumulatorsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"$ref\": \"#/components/schemas/JobVertexID\"\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"subtasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskAccumulatorsInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtasks-all-accumulators-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtasksAllAccumulatorsInfo
---
