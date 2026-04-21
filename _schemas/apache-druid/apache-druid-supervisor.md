---
description: An Apache Druid supervisor for managing continuous streaming data ingestion from Kafka or Kinesis.
layout: schema
name: Supervisor
properties_list:
- description: Supervisor ID (same as datasource name by convention).
  name: id
  type: string
- description: Supervisor operational state.
  name: state
  type: string
- description: Supervisor health status.
  name: healthStatus
  type: string
- description: Detailed supervisor sub-state.
  name: detailedState
  type: string
- description: Full supervisor spec including ioConfig and tuningConfig.
  name: spec
  type: object
- description: When the last task completed.
  name: lastTaskCompletionTime
  type: string
- description: Number of currently active ingestion tasks.
  name: activeTasks
  type: integer
- description: Number of tasks publishing segments.
  name: publishingTasks
  type: integer
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-supervisor-schema.json
slug: apache-druid-supervisor
tags:
- Analytics
- Apache
- Database
- Kafka
- OLAP
- Open Source
- Real-Time
- SQL
- Time Series
title: Supervisor
---
