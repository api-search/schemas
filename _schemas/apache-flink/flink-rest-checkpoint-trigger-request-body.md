---
description: CheckpointTriggerRequestBody schema from Apache Flink REST API
layout: schema
name: CheckpointTriggerRequestBody
properties_list:
- description: ''
  name: checkpointType
  type: object
- description: ''
  name: triggerId
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-trigger-request-body-schema.json
slug: flink-rest-checkpoint-trigger-request-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-trigger-request-body-schema.json\",\n  \"title\": \"CheckpointTriggerRequestBody\",\n  \"description\": \"CheckpointTriggerRequestBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkpointType\": {\n      \"$ref\": \"#/components/schemas/CheckpointType\"\n    },\n    \"triggerId\": {\n      \"$ref\": \"#/components/schemas/TriggerId\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-trigger-request-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointTriggerRequestBody
---
