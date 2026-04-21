---
description: Request to stop a SeaTunnel job
layout: schema
name: JobStopRequest
properties_list:
- description: Job identifier to stop
  name: jobId
  type: string
- description: Whether to create a savepoint before stopping
  name: isStopWithSavePoint
  type: boolean
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-stop-request-schema.json
slug: apache-seatunnel-job-stop-request
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobStopRequest
---
