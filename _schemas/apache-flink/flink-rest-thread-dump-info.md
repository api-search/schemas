---
description: ThreadDumpInfo schema from Apache Flink REST API
layout: schema
name: ThreadDumpInfo
properties_list:
- description: ''
  name: threadInfos
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-thread-dump-info-schema.json
slug: flink-rest-thread-dump-info
source_filename: flink-rest-thread-dump-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-thread-dump-info-schema.json\",\n  \"title\": \"ThreadDumpInfo\",\n  \"description\": \"ThreadDumpInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threadInfos\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ThreadInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-thread-dump-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ThreadDumpInfo
---
