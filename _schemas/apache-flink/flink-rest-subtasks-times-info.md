---
description: SubtasksTimesInfo schema from Apache Flink REST API
layout: schema
name: SubtasksTimesInfo
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: now
  type: integer
- description: ''
  name: subtasks
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-subtasks-times-info-schema.json
slug: flink-rest-subtasks-times-info
source_filename: flink-rest-subtasks-times-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtasks-times-info-schema.json\",\n  \"title\": \"SubtasksTimesInfo\",\n  \"description\": \"SubtasksTimesInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"now\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"subtasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubtaskTimeInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-subtasks-times-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SubtasksTimesInfo
---
