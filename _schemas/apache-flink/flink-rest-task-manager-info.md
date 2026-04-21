---
description: TaskManagerInfo schema from Apache Flink REST API
layout: schema
name: TaskManagerInfo
properties_list:
- description: ''
  name: blocked
  type: boolean
- description: ''
  name: dataPort
  type: integer
- description: ''
  name: freeResource
  type: object
- description: ''
  name: freeSlots
  type: integer
- description: ''
  name: hardware
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: jmxPort
  type: integer
- description: ''
  name: memoryConfiguration
  type: object
- description: ''
  name: path
  type: string
- description: ''
  name: slotsNumber
  type: integer
- description: ''
  name: timeSinceLastHeartbeat
  type: integer
- description: ''
  name: totalResource
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-task-manager-info-schema.json
slug: flink-rest-task-manager-info
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: TaskManagerInfo
---
