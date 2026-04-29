---
description: SavepointTriggerRequestBody schema from Apache Flink REST API
layout: schema
name: SavepointTriggerRequestBody
properties_list:
- description: ''
  name: cancel-job
  type: boolean
- description: ''
  name: formatType
  type: object
- description: ''
  name: target-directory
  type: string
- description: ''
  name: triggerId
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-savepoint-trigger-request-body-schema.json
slug: flink-rest-savepoint-trigger-request-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-savepoint-trigger-request-body-schema.json\",\n  \"title\": \"SavepointTriggerRequestBody\",\n  \"description\": \"SavepointTriggerRequestBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cancel-job\": {\n      \"type\": \"boolean\"\n    },\n    \"formatType\": {\n      \"$ref\": \"#/components/schemas/SavepointFormatType\"\n    },\n    \"target-directory\": {\n      \"type\": \"string\"\n    },\n    \"triggerId\": {\n      \"$ref\": \"#/components/schemas/TriggerId\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-savepoint-trigger-request-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SavepointTriggerRequestBody
---
