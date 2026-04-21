---
description: Request to submit a SeaTunnel job
layout: schema
name: JobSubmitRequest
properties_list:
- description: SeaTunnel job configuration in JSON or HOCON format
  name: jobContent
  type: string
- description: Optional job name
  name: jobName
  type: string
- description: Whether to start from a savepoint
  name: isStartWithSavePoint
  type: boolean
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-submit-request-schema.json
slug: apache-seatunnel-job-submit-request
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobSubmitRequest
---
