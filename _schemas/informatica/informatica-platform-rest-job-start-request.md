---
description: Request body for starting a job. You can identify the task by taskId or taskName, and must specify the task type.
layout: schema
name: JobStartRequest
properties_list:
- description: The resource type identifier. Must be set to "job".
  name: '@type'
  type: string
- description: The ID of the task to run. Either taskId or taskName must be provided.
  name: taskId
  type: string
- description: The name of the task to run. Either taskId or taskName must be provided.
  name: taskName
  type: string
- description: The type of the task to run. Supported values include MTT (mapping task), WORKFLOW (taskflow), DSS (synchronization task), DRS (data replication task), and PCS (PowerCenter task).
  name: taskType
  type: string
- description: An optional URL that receives a callback when the job completes.
  name: callbackUrl
  type: string
- description: Optional runtime configuration for the job execution.
  name: runtime
  type: object
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-job-start-request-schema.json
slug: informatica-platform-rest-job-start-request
source_filename: informatica-platform-rest-job-start-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobStartRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for starting a job. You can identify the task by taskId or taskName, and must specify the task type.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier. Must be set to \\\"job\\\".\"\n    },\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the task to run. Either taskId or taskName must be provided.\"\n    },\n    \"taskName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task to run. Either taskId or taskName must be provided.\"\n    },\n    \"taskType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the task to run. Supported values include MTT (mapping task), WORKFLOW (taskflow), DSS (synchronization task), DRS (data replication task), and PCS (PowerCenter\
  \ task).\"\n    },\n    \"callbackUrl\": {\n      \"type\": \"string\",\n      \"description\": \"An optional URL that receives a callback when the job completes.\"\n    },\n    \"runtime\": {\n      \"type\": \"object\",\n      \"description\": \"Optional runtime configuration for the job execution.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-job-start-request-schema.json
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
title: JobStartRequest
---
