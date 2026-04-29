---
description: CheckpointStatisticsSummary schema from Apache Flink REST API
layout: schema
name: CheckpointStatisticsSummary
properties_list:
- description: ''
  name: alignment_buffered
  type: object
- description: ''
  name: checkpointed_size
  type: object
- description: ''
  name: end_to_end_duration
  type: object
- description: ''
  name: persisted_data
  type: object
- description: ''
  name: processed_data
  type: object
- description: ''
  name: state_size
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-statistics-summary-schema.json
slug: flink-rest-checkpoint-statistics-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-statistics-summary-schema.json\",\n  \"title\": \"CheckpointStatisticsSummary\",\n  \"description\": \"CheckpointStatisticsSummary schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alignment_buffered\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"checkpointed_size\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"end_to_end_duration\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"persisted_data\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"processed_data\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"state_size\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-checkpoint-statistics-summary-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointStatisticsSummary
---
