---
description: EnvironmentInfo schema from Apache Flink REST API
layout: schema
name: EnvironmentInfo
properties_list:
- description: ''
  name: classpath
  type: array
- description: ''
  name: jvm
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-environment-info-schema.json
slug: flink-rest-environment-info
source_filename: flink-rest-environment-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-environment-info-schema.json\",\n  \"title\": \"EnvironmentInfo\",\n  \"description\": \"EnvironmentInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classpath\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jvm\": {\n      \"$ref\": \"#/components/schemas/JVMInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-environment-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: EnvironmentInfo
---
