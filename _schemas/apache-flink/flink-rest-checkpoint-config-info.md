---
description: CheckpointConfigInfo schema from Apache Flink REST API
layout: schema
name: CheckpointConfigInfo
properties_list:
- description: ''
  name: aligned_checkpoint_timeout
  type: integer
- description: ''
  name: changelog_periodic_materialization_interval
  type: integer
- description: ''
  name: changelog_storage
  type: string
- description: ''
  name: checkpoint_storage
  type: string
- description: ''
  name: checkpoints_after_tasks_finish
  type: boolean
- description: ''
  name: externalization
  type: object
- description: ''
  name: interval
  type: integer
- description: ''
  name: max_concurrent
  type: integer
- description: ''
  name: min_pause
  type: integer
- description: ''
  name: mode
  type: object
- description: ''
  name: state_backend
  type: string
- description: ''
  name: state_changelog_enabled
  type: boolean
- description: ''
  name: timeout
  type: integer
- description: ''
  name: tolerable_failed_checkpoints
  type: integer
- description: ''
  name: unaligned_checkpoints
  type: boolean
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-checkpoint-config-info-schema.json
slug: flink-rest-checkpoint-config-info
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: CheckpointConfigInfo
---
