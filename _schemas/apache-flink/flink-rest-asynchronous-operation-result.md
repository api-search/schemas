---
description: AsynchronousOperationResult schema from Apache Flink REST API
layout: schema
name: AsynchronousOperationResult
properties_list:
- description: ''
  name: operation
  type: object
- description: ''
  name: status
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-asynchronous-operation-result-schema.json
slug: flink-rest-asynchronous-operation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-asynchronous-operation-result-schema.json\",\n  \"title\": \"AsynchronousOperationResult\",\n  \"description\": \"AsynchronousOperationResult schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AsynchronousOperationInfo\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckpointInfo\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SavepointInfo\"\n        }\n      ]\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/QueueStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-asynchronous-operation-result-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: AsynchronousOperationResult
---
