---
description: GarbageCollectorInfo schema from Apache Flink REST API
layout: schema
name: GarbageCollectorInfo
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: time
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-garbage-collector-info-schema.json
slug: flink-rest-garbage-collector-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-garbage-collector-info-schema.json\",\n  \"title\": \"GarbageCollectorInfo\",\n  \"description\": \"GarbageCollectorInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-garbage-collector-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: GarbageCollectorInfo
---
