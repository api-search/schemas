---
description: Counts schema from Apache Flink REST API
layout: schema
name: Counts
properties_list:
- description: ''
  name: completed
  type: integer
- description: ''
  name: failed
  type: integer
- description: ''
  name: in_progress
  type: integer
- description: ''
  name: restored
  type: integer
- description: ''
  name: total
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-counts-schema.json
slug: flink-rest-counts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-counts-schema.json\",\n  \"title\": \"Counts\",\n  \"description\": \"Counts schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"completed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"failed\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"in_progress\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"restored\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-counts-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: Counts
---
