---
description: LogListInfo schema from Apache Flink REST API
layout: schema
name: LogListInfo
properties_list:
- description: ''
  name: logs
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-log-list-info-schema.json
slug: flink-rest-log-list-info
source_filename: flink-rest-log-list-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-log-list-info-schema.json\",\n  \"title\": \"LogListInfo\",\n  \"description\": \"LogListInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-log-list-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: LogListInfo
---
