---
description: High-level cluster overview
layout: schema
name: ClusterOverview
properties_list:
- description: Number of worker nodes
  name: workers
  type: integer
- description: Number of running jobs
  name: runningJobs
  type: integer
- description: Number of finished jobs
  name: finishedJobs
  type: integer
- description: Number of failed jobs
  name: failedJobs
  type: integer
- description: Number of canceled jobs
  name: canceledJobs
  type: integer
- description: Total available task slots
  name: totalSlot
  type: integer
- description: Currently used task slots
  name: usedSlot
  type: integer
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-cluster-overview-schema.json
slug: apache-seatunnel-cluster-overview
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: ClusterOverview
---
