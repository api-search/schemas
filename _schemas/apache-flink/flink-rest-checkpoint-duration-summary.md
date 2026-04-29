---
description: CheckpointDurationSummary schema from Apache Flink REST API
layout: schema
name: CheckpointDurationSummary
properties_list:
- description: ''
  name: async
  type: object
- description: ''
  name: sync
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-duration-summary-schema.json
slug: flink-rest-checkpoint-duration-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-duration-summary-schema.json\",\n  \"title\": \"CheckpointDurationSummary\",\n  \"description\": \"CheckpointDurationSummary schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"async\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"sync\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-duration-summary-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointDurationSummary
---
