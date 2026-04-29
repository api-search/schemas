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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-metrics-schema.json\",\n  \"title\": \"JobMetrics\",\n  \"description\": \"Runtime metrics for a SeaTunnel job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceReceivedCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total records read from source\"\n    },\n    \"sinkWriteCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total records written to sink\"\n    },\n    \"sourceReceivedQPS\": {\n      \"type\": \"number\",\n      \"description\": \"Records per second from source\"\n    },\n    \"sinkWriteQPS\": {\n      \"type\": \"number\",\n      \"description\": \"Records per second to sink\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-metrics-schema.json
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
