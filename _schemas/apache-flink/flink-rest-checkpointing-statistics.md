---
description: CheckpointingStatistics schema from Apache Flink REST API
layout: schema
name: CheckpointingStatistics
properties_list:
- description: ''
  name: counts
  type: object
- description: ''
  name: history
  type: array
- description: ''
  name: latest
  type: object
- description: ''
  name: summary
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpointing-statistics-schema.json
slug: flink-rest-checkpointing-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpointing-statistics-schema.json\",\n  \"title\": \"CheckpointingStatistics\",\n  \"description\": \"CheckpointingStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"counts\": {\n      \"$ref\": \"#/components/schemas/Counts\"\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CheckpointStatistics\"\n      }\n    },\n    \"latest\": {\n      \"$ref\": \"#/components/schemas/LatestCheckpoints\"\n    },\n    \"summary\": {\n      \"$ref\": \"#/components/schemas/CheckpointStatisticsSummary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpointing-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointingStatistics
---
