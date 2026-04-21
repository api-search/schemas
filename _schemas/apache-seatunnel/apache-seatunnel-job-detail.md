---
description: Detailed information about a SeaTunnel job
layout: schema
name: JobDetail
properties_list:
- description: ''
  name: jobId
  type: string
- description: ''
  name: jobName
  type: string
- description: ''
  name: jobStatus
  type: string
- description: Job DAG definition
  name: jobDag
  type: object
- description: ''
  name: metrics
  type: object
- description: ''
  name: createTime
  type: string
- description: ''
  name: finishTime
  type: string
- description: Error message if job failed
  name: errorMsg
  type: string
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-detail-schema.json
slug: apache-seatunnel-job-detail
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobDetail
---
