---
description: TaskCheckpointStatisticsWithSubtaskDetailsSummary schema from Apache Flink REST API
layout: schema
name: TaskCheckpointStatisticsWithSubtaskDetailsSummary
properties_list:
- description: ''
  name: alignment
  type: object
- description: ''
  name: checkpoint_duration
  type: object
- description: ''
  name: checkpointed_size
  type: object
- description: ''
  name: end_to_end_duration
  type: object
- description: ''
  name: start_delay
  type: object
- description: ''
  name: state_size
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-checkpoint-statistics-with-subtask-details-summary-schema.json
slug: flink-rest-task-checkpoint-statistics-with-subtask-details-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-checkpoint-statistics-with-subtask-details-summary-schema.json\",\n  \"title\": \"TaskCheckpointStatisticsWithSubtaskDetailsSummary\",\n  \"description\": \"TaskCheckpointStatisticsWithSubtaskDetailsSummary schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alignment\": {\n      \"$ref\": \"#/components/schemas/CheckpointAlignmentSummary\"\n    },\n    \"checkpoint_duration\": {\n      \"$ref\": \"#/components/schemas/CheckpointDurationSummary\"\n    },\n    \"checkpointed_size\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"end_to_end_duration\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"start_delay\": {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    },\n    \"state_size\"\
  : {\n      \"$ref\": \"#/components/schemas/StatsSummaryDto\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-task-checkpoint-statistics-with-subtask-details-summary-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskCheckpointStatisticsWithSubtaskDetailsSummary
---
