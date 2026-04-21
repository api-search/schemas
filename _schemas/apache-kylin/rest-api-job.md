---
description: A Kylin build job
layout: schema
name: Job
properties_list:
- description: ''
  name: uuid
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: relatedCube
  type: string
- description: ''
  name: relatedSegment
  type: string
- description: ''
  name: status
  type: string
- description: Submit time as Unix timestamp
  name: submitTime
  type: integer
- description: Job duration in seconds
  name: duration
  type: integer
- description: MapReduce waiting time
  name: mrWaiting
  type: integer
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-job-schema.json
slug: rest-api-job
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: Job
---
