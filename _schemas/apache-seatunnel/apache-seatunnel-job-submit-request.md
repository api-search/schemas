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
source_filename: apache-seatunnel-job-submit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-submit-request-schema.json\",\n  \"title\": \"JobSubmitRequest\",\n  \"description\": \"Request to submit a SeaTunnel job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobContent\": {\n      \"type\": \"string\",\n      \"description\": \"SeaTunnel job configuration in JSON or HOCON format\"\n    },\n    \"jobName\": {\n      \"type\": \"string\",\n      \"description\": \"Optional job name\"\n    },\n    \"isStartWithSavePoint\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to start from a savepoint\"\n    }\n  },\n  \"required\": [\n    \"jobContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-job-submit-request-schema.json
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
