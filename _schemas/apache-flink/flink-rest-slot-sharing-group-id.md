---
description: SlotSharingGroupId schema from Apache Flink REST API
layout: schema
name: SlotSharingGroupId
properties_list:
- description: ''
  name: bytes
  type: array
- description: ''
  name: lowerPart
  type: integer
- description: ''
  name: upperPart
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-slot-sharing-group-id-schema.json
slug: flink-rest-slot-sharing-group-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-slot-sharing-group-id-schema.json\",\n  \"title\": \"SlotSharingGroupId\",\n  \"description\": \"SlotSharingGroupId schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bytes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"byte\"\n      }\n    },\n    \"lowerPart\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"upperPart\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-slot-sharing-group-id-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SlotSharingGroupId
---
