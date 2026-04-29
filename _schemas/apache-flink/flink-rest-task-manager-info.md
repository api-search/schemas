---
description: TaskManagerInfo schema from Apache Flink REST API
layout: schema
name: TaskManagerInfo
properties_list:
- description: ''
  name: blocked
  type: boolean
- description: ''
  name: dataPort
  type: integer
- description: ''
  name: freeResource
  type: object
- description: ''
  name: freeSlots
  type: integer
- description: ''
  name: hardware
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: jmxPort
  type: integer
- description: ''
  name: memoryConfiguration
  type: object
- description: ''
  name: path
  type: string
- description: ''
  name: slotsNumber
  type: integer
- description: ''
  name: timeSinceLastHeartbeat
  type: integer
- description: ''
  name: totalResource
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-manager-info-schema.json
slug: flink-rest-task-manager-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-manager-info-schema.json\",\n  \"title\": \"TaskManagerInfo\",\n  \"description\": \"TaskManagerInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blocked\": {\n      \"type\": \"boolean\"\n    },\n    \"dataPort\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"freeResource\": {\n      \"$ref\": \"#/components/schemas/ResourceProfileInfo\"\n    },\n    \"freeSlots\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"hardware\": {\n      \"$ref\": \"#/components/schemas/HardwareDescription\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/ResourceID\"\n    },\n    \"jmxPort\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"memoryConfiguration\": {\n\
  \      \"$ref\": \"#/components/schemas/TaskExecutorMemoryConfiguration\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"slotsNumber\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"timeSinceLastHeartbeat\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"totalResource\": {\n      \"$ref\": \"#/components/schemas/ResourceProfileInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-manager-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskManagerInfo
---
