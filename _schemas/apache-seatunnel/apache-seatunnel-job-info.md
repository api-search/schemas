---
description: Summary info for a SeaTunnel job
layout: schema
name: JobInfo
properties_list:
- description: Job identifier
  name: jobId
  type: string
- description: Job name
  name: jobName
  type: string
- description: Current job status
  name: jobStatus
  type: string
- description: ''
  name: createTime
  type: string
- description: ''
  name: finishTime
  type: string
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-job-info-schema.json
slug: apache-seatunnel-job-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-info-schema.json\",\n  \"title\": \"JobInfo\",\n  \"description\": \"Summary info for a SeaTunnel job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job identifier\"\n    },\n    \"jobName\": {\n      \"type\": \"string\",\n      \"description\": \"Job name\"\n    },\n    \"jobStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RUNNING\",\n        \"FINISHED\",\n        \"FAILED\",\n        \"CANCELED\",\n        \"CANCELLING\"\n      ],\n      \"description\": \"Current job status\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-info-schema.json
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: JobInfo
---
