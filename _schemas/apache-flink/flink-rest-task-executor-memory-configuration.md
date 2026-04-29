---
description: TaskExecutorMemoryConfiguration schema from Apache Flink REST API
layout: schema
name: TaskExecutorMemoryConfiguration
properties_list:
- description: ''
  name: frameworkHeap
  type: integer
- description: ''
  name: frameworkOffHeap
  type: integer
- description: ''
  name: jvmMetaspace
  type: integer
- description: ''
  name: jvmOverhead
  type: integer
- description: ''
  name: managedMemory
  type: integer
- description: ''
  name: networkMemory
  type: integer
- description: ''
  name: taskHeap
  type: integer
- description: ''
  name: taskOffHeap
  type: integer
- description: ''
  name: totalFlinkMemory
  type: integer
- description: ''
  name: totalProcessMemory
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-executor-memory-configuration-schema.json
slug: flink-rest-task-executor-memory-configuration
source_filename: flink-rest-task-executor-memory-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-executor-memory-configuration-schema.json\",\n  \"title\": \"TaskExecutorMemoryConfiguration\",\n  \"description\": \"TaskExecutorMemoryConfiguration schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frameworkHeap\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"frameworkOffHeap\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"jvmMetaspace\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"jvmOverhead\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"managedMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"networkMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"taskHeap\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"taskOffHeap\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"totalFlinkMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"totalProcessMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-executor-memory-configuration-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskExecutorMemoryConfiguration
---
