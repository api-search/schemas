---
description: CheckpointStatistics schema from Apache Flink REST API
layout: schema
name: CheckpointStatistics
properties_list:
- description: ''
  name: alignment_buffered
  type: integer
- description: ''
  name: checkpoint_type
  type: object
- description: ''
  name: checkpointed_size
  type: integer
- description: ''
  name: className
  type: string
- description: ''
  name: end_to_end_duration
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: is_savepoint
  type: boolean
- description: ''
  name: latest_ack_timestamp
  type: integer
- description: ''
  name: num_acknowledged_subtasks
  type: integer
- description: ''
  name: num_subtasks
  type: integer
- description: ''
  name: persisted_data
  type: integer
- description: ''
  name: processed_data
  type: integer
- description: ''
  name: savepointFormat
  type: string
- description: ''
  name: state_size
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: tasks
  type: object
- description: ''
  name: trigger_timestamp
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-statistics-schema.json
slug: flink-rest-checkpoint-statistics
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointStatistics
---
