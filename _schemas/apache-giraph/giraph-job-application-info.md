---
description: YARN application (Giraph job) status information
layout: schema
name: ApplicationInfo
properties_list:
- description: YARN application ID
  name: id
  type: string
- description: Application name (usually Giraph followed by the algorithm name)
  name: name
  type: string
- description: Application type (MAPREDUCE for Giraph)
  name: applicationType
  type: string
- description: Current application state
  name: state
  type: string
- description: Final status after completion
  name: finalStatus
  type: string
- description: Job completion percentage (0-100)
  name: progress
  type: number
- description: URL for job tracking UI
  name: trackingUrl
  type: string
- description: YARN queue name
  name: queue
  type: string
- description: Job start time in milliseconds since epoch
  name: startedTime
  type: integer
- description: Job finish time in milliseconds (0 if still running)
  name: finishedTime
  type: integer
- description: Elapsed time in milliseconds
  name: elapsedTime
  type: integer
- description: Number of running containers
  name: numContainers
  type: integer
provider_name: Apache Giraph
provider_slug: apache-giraph
schema_file: json-schema/giraph-job-application-info-schema.json
slug: giraph-job-application-info
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
title: ApplicationInfo
---
