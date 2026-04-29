---
description: SlotInfo schema from Apache Flink REST API
layout: schema
name: SlotInfo
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: resource
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-slot-info-schema.json
slug: flink-rest-slot-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-slot-info-schema.json\",\n  \"title\": \"SlotInfo\",\n  \"description\": \"SlotInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"$ref\": \"#/components/schemas/JobID\"\n    },\n    \"resource\": {\n      \"$ref\": \"#/components/schemas/ResourceProfileInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-slot-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: SlotInfo
---
