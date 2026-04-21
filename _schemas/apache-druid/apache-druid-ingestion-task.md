---
description: An Apache Druid data ingestion task for batch or streaming data loading.
layout: schema
name: IngestionTask
properties_list:
- description: Unique task ID assigned by Druid.
  name: id
  type: string
- description: Task type identifier.
  name: type
  type: string
- description: Target datasource name.
  name: dataSource
  type: string
- description: Task group ID for parallel tasks.
  name: groupId
  type: string
- description: Current task status.
  name: status
  type: string
- description: Task creation timestamp.
  name: createdTime
  type: string
- description: Task queue insertion timestamp.
  name: queueInsertionTime
  type: string
- description: Host and port where this task is running.
  name: location
  type: object
- description: Task duration in milliseconds (-1 if still running).
  name: duration
  type: integer
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-ingestion-task-schema.json
slug: apache-druid-ingestion-task
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
title: IngestionTask
---
