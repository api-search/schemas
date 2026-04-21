---
description: Runtime metrics for a SeaTunnel job
layout: schema
name: JobMetrics
properties_list:
- description: Total records read from source
  name: sourceReceivedCount
  type: integer
- description: Total records written to sink
  name: sinkWriteCount
  type: integer
- description: Records per second from source
  name: sourceReceivedQPS
  type: number
- description: Records per second to sink
  name: sinkWriteQPS
  type: number
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-metrics-schema.json
slug: apache-seatunnel-job-metrics
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobMetrics
---
