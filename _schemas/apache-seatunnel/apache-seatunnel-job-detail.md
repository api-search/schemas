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
source_filename: apache-seatunnel-job-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-detail-schema.json\",\n  \"title\": \"JobDetail\",\n  \"description\": \"Detailed information about a SeaTunnel job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\"\n    },\n    \"jobName\": {\n      \"type\": \"string\"\n    },\n    \"jobStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RUNNING\",\n        \"FINISHED\",\n        \"FAILED\",\n        \"CANCELED\",\n        \"CANCELLING\"\n      ]\n    },\n    \"jobDag\": {\n      \"type\": \"object\",\n      \"description\": \"Job DAG definition\"\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/JobMetrics\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finishTime\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\"\n    },\n    \"errorMsg\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if job failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-detail-schema.json
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
