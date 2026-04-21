---
description: Rest representation of org.apache.ignite.compute.JobState.
layout: schema
name: JobState
properties_list:
- description: Job ID.
  name: id
  type: string
- description: Job status.
  name: status
  type: object
- description: Job create time.
  name: createTime
  type: string
- description: Job start time.
  name: startTime
  type: string
- description: Job finish time.
  name: finishTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-job-state-schema.json
slug: rest-api-job-state
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: JobState
---
