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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-stop-request-schema.json\",\n  \"title\": \"JobStopRequest\",\n  \"description\": \"Request to stop a SeaTunnel job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job identifier to stop\"\n    },\n    \"isStopWithSavePoint\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create a savepoint before stopping\"\n    }\n  },\n  \"required\": [\n    \"jobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-stop-request-schema.json
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
