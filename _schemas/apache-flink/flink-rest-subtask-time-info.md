---
description: SubtaskTimeInfo schema from Apache Flink REST API
layout: schema
name: SubtaskTimeInfo
properties_list:
- description: ''
  name: duration
  type: integer
- description: ''
  name: endpoint
  type: string
- description: ''
  name: subtask
  type: integer
- description: ''
  name: timestamps
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtask-time-info-schema.json
slug: flink-rest-subtask-time-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-time-info-schema.json\",\n  \"title\": \"SubtaskTimeInfo\",\n  \"description\": \"SubtaskTimeInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"subtask\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"timestamps\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtask-time-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtaskTimeInfo
---
