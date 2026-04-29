---
description: IOMetricsInfo schema from Apache Flink REST API
layout: schema
name: IOMetricsInfo
properties_list:
- description: ''
  name: accumulated-backpressured-time
  type: integer
- description: ''
  name: accumulated-busy-time
  type: number
- description: ''
  name: accumulated-idle-time
  type: integer
- description: ''
  name: read-bytes
  type: integer
- description: ''
  name: read-bytes-complete
  type: boolean
- description: ''
  name: read-records
  type: integer
- description: ''
  name: read-records-complete
  type: boolean
- description: ''
  name: write-bytes
  type: integer
- description: ''
  name: write-bytes-complete
  type: boolean
- description: ''
  name: write-records
  type: integer
- description: ''
  name: write-records-complete
  type: boolean
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-io-metrics-info-schema.json
slug: flink-rest-io-metrics-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-io-metrics-info-schema.json\",\n  \"title\": \"IOMetricsInfo\",\n  \"description\": \"IOMetricsInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accumulated-backpressured-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"accumulated-busy-time\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"accumulated-idle-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"read-bytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"read-bytes-complete\": {\n      \"type\": \"boolean\"\n    },\n    \"read-records\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"read-records-complete\": {\n      \"type\": \"boolean\"\
  \n    },\n    \"write-bytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"write-bytes-complete\": {\n      \"type\": \"boolean\"\n    },\n    \"write-records\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"write-records-complete\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-io-metrics-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: IOMetricsInfo
---
