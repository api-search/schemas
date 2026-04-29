---
description: CheckpointAlignmentSummary schema from Apache Flink REST API
layout: schema
name: CheckpointAlignmentSummary
properties_list:
- description: ''
  name: buffered
  type: object
- description: ''
  name: duration
  type: object
- description: ''
  name: persisted
  type: object
- description: ''
  name: processed
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-alignment-summary-schema.json
slug: flink-rest-checkpoint-alignment-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-alignment-summary-schema.json\",\n  \"title\": \"CheckpointAlignmentSummary\",\n  \"description\": \"CheckpointAlignmentSummary schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buffered\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"duration\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"persisted\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"processed\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-alignment-summary-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointAlignmentSummary
---
