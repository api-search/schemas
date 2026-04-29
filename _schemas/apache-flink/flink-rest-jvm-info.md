---
description: JVMInfo schema from Apache Flink REST API
layout: schema
name: JVMInfo
properties_list:
- description: ''
  name: arch
  type: string
- description: ''
  name: options
  type: array
- description: ''
  name: version
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-jvm-info-schema.json
slug: flink-rest-jvm-info
source_filename: flink-rest-jvm-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jvm-info-schema.json\",\n  \"title\": \"JVMInfo\",\n  \"description\": \"JVMInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arch\": {\n      \"type\": \"string\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jvm-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JVMInfo
---
