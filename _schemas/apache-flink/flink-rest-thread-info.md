---
description: ThreadInfo schema from Apache Flink REST API
layout: schema
name: ThreadInfo
properties_list:
- description: ''
  name: stringifiedThreadInfo
  type: string
- description: ''
  name: threadName
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-thread-info-schema.json
slug: flink-rest-thread-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-thread-info-schema.json\",\n  \"title\": \"ThreadInfo\",\n  \"description\": \"ThreadInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stringifiedThreadInfo\": {\n      \"type\": \"string\"\n    },\n    \"threadName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-thread-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ThreadInfo
---
