---
description: Configuration and state of a Routine Load job that continuously ingests data from Apache Kafka into Doris.
layout: schema
name: RoutineLoadJob
properties_list:
- description: Routine Load job ID.
  name: id
  type: integer
- description: Name of the Routine Load job.
  name: name
  type: string
- description: Target database name.
  name: dbName
  type: string
- description: Target table name.
  name: tableName
  type: string
- description: Current state of the load job.
  name: state
  type: string
- description: Data source type.
  name: dataSourceType
  type: string
- description: Kafka broker list.
  name: kafkaBrokerList
  type: string
- description: Kafka topic to consume from.
  name: kafkaTopic
  type: string
- description: Data format.
  name: format
  type: string
- description: Total number of rows loaded since job start.
  name: totalRows
  type: integer
- description: Number of rows successfully loaded.
  name: loadedRows
  type: integer
- description: Number of rows filtered.
  name: filteredRows
  type: integer
- description: Job creation time.
  name: createTime
  type: string
provider_name: Apache Doris
provider_slug: apache-doris
schema_file: json-schema/apache-doris-routine-load-job-schema.json
slug: apache-doris-routine-load-job
tags:
- Analytics
- Apache
- Database
- Lakehouse
- MPP
- OLAP
- Open Source
- Real-Time
- SQL
title: RoutineLoadJob
---
