---
description: TaskManagerMetricsInfo schema from Apache Flink REST API
layout: schema
name: TaskManagerMetricsInfo
properties_list:
- description: ''
  name: directCount
  type: integer
- description: ''
  name: directMax
  type: integer
- description: ''
  name: directUsed
  type: integer
- description: ''
  name: garbageCollectors
  type: array
- description: ''
  name: heapCommitted
  type: integer
- description: ''
  name: heapMax
  type: integer
- description: ''
  name: heapUsed
  type: integer
- description: ''
  name: mappedCount
  type: integer
- description: ''
  name: mappedMax
  type: integer
- description: ''
  name: mappedUsed
  type: integer
- description: ''
  name: nettyShuffleMemoryAvailable
  type: integer
- description: ''
  name: nettyShuffleMemorySegmentsAvailable
  type: integer
- description: ''
  name: nettyShuffleMemorySegmentsTotal
  type: integer
- description: ''
  name: nettyShuffleMemorySegmentsUsed
  type: integer
- description: ''
  name: nettyShuffleMemoryTotal
  type: integer
- description: ''
  name: nettyShuffleMemoryUsed
  type: integer
- description: ''
  name: nonHeapCommitted
  type: integer
- description: ''
  name: nonHeapMax
  type: integer
- description: ''
  name: nonHeapUsed
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-manager-metrics-info-schema.json
slug: flink-rest-task-manager-metrics-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-manager-metrics-info-schema.json\",\n  \"title\": \"TaskManagerMetricsInfo\",\n  \"description\": \"TaskManagerMetricsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"directMax\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"directUsed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"garbageCollectors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GarbageCollectorInfo\"\n      }\n    },\n    \"heapCommitted\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"heapMax\": {\n      \"type\": \"integer\",\n      \"format\": \"\
  int64\"\n    },\n    \"heapUsed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"mappedCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"mappedMax\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"mappedUsed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemoryAvailable\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemorySegmentsAvailable\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemorySegmentsTotal\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemorySegmentsUsed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemoryTotal\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nettyShuffleMemoryUsed\": {\n      \"type\": \"integer\",\n      \"format\"\
  : \"int64\"\n    },\n    \"nonHeapCommitted\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nonHeapMax\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"nonHeapUsed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-manager-metrics-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskManagerMetricsInfo
---
