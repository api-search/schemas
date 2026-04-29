---
description: SavepointInfo schema from Apache Flink REST API
layout: schema
name: SavepointInfo
properties_list:
- description: ''
  name: failure-cause
  type: object
- description: ''
  name: location
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-savepoint-info-schema.json
slug: flink-rest-savepoint-info
source_filename: flink-rest-savepoint-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-savepoint-info-schema.json\",\n  \"title\": \"SavepointInfo\",\n  \"description\": \"SavepointInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failure-cause\": {\n      \"$ref\": \"#/components/schemas/SerializedThrowable\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-savepoint-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SavepointInfo
---
