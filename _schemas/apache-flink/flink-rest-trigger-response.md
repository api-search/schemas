---
description: TriggerResponse schema from Apache Flink REST API
layout: schema
name: TriggerResponse
properties_list:
- description: ''
  name: request-id
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-trigger-response-schema.json
slug: flink-rest-trigger-response
source_filename: flink-rest-trigger-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-trigger-response-schema.json\",\n  \"title\": \"TriggerResponse\",\n  \"description\": \"TriggerResponse schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request-id\": {\n      \"$ref\": \"#/components/schemas/TriggerId\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-trigger-response-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TriggerResponse
---
