---
description: Response returned when a job is successfully started.
layout: schema
name: JobStartResponse
properties_list:
- description: The ID of the task that was started.
  name: taskId
  type: string
- description: The type of the task.
  name: taskType
  type: string
- description: The unique run ID for this job execution. Use this ID to track job status.
  name: runId
  type: integer
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-job-start-response-schema.json
slug: informatica-platform-rest-job-start-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobStartResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response returned when a job is successfully started.\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the task that was started.\"\n    },\n    \"taskType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the task.\"\n    },\n    \"runId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique run ID for this job execution. Use this ID to track job status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-job-start-response-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: JobStartResponse
---
