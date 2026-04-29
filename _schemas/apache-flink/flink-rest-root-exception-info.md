---
description: RootExceptionInfo schema from Apache Flink REST API
layout: schema
name: RootExceptionInfo
properties_list:
- description: ''
  name: concurrentExceptions
  type: array
- description: ''
  name: endpoint
  type: string
- description: ''
  name: exceptionName
  type: string
- description: ''
  name: failureLabels
  type: object
- description: ''
  name: stacktrace
  type: string
- description: ''
  name: taskManagerId
  type: string
- description: ''
  name: taskName
  type: string
- description: ''
  name: timestamp
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-root-exception-info-schema.json
slug: flink-rest-root-exception-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-root-exception-info-schema.json\",\n  \"title\": \"RootExceptionInfo\",\n  \"description\": \"RootExceptionInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"concurrentExceptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExceptionInfo\"\n      }\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"exceptionName\": {\n      \"type\": \"string\"\n    },\n    \"failureLabels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"stacktrace\": {\n      \"type\": \"string\"\n    },\n    \"taskManagerId\": {\n      \"type\": \"string\"\n    },\n    \"taskName\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\":\
  \ {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-root-exception-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: RootExceptionInfo
---
