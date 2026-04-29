---
description: ExecutionConfigInfo schema from Apache Flink REST API
layout: schema
name: ExecutionConfigInfo
properties_list:
- description: ''
  name: job-parallelism
  type: integer
- description: ''
  name: object-reuse-mode
  type: boolean
- description: ''
  name: restart-strategy
  type: string
- description: ''
  name: user-config
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-execution-config-info-schema.json
slug: flink-rest-execution-config-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-execution-config-info-schema.json\",\n  \"title\": \"ExecutionConfigInfo\",\n  \"description\": \"ExecutionConfigInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job-parallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"object-reuse-mode\": {\n      \"type\": \"boolean\"\n    },\n    \"restart-strategy\": {\n      \"type\": \"string\"\n    },\n    \"user-config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-execution-config-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ExecutionConfigInfo
---
