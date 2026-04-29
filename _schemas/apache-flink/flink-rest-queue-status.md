---
description: QueueStatus schema from Apache Flink REST API
layout: schema
name: QueueStatus
properties_list:
- description: ''
  name: id
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-queue-status-schema.json
slug: flink-rest-queue-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-queue-status-schema.json\",\n  \"title\": \"QueueStatus\",\n  \"description\": \"QueueStatus schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-queue-status-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: QueueStatus
---
