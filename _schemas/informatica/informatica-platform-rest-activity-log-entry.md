---
description: An entry in the activity log representing the execution status of a job.
layout: schema
name: ActivityLogEntry
properties_list:
- description: The activity log entry ID.
  name: id
  type: string
- description: The type of activity.
  name: type
  type: string
- description: The ID of the task or object.
  name: objectId
  type: string
- description: The name of the task or object.
  name: objectName
  type: string
- description: The job run ID.
  name: runId
  type: integer
- description: The Secure Agent that ran the job.
  name: agentId
  type: string
- description: The runtime environment used.
  name: runtimeEnvironmentId
  type: string
- description: The time the job started.
  name: startTime
  type: string
- description: The time the job completed.
  name: endTime
  type: string
- description: The job execution state. Common values are 1 (success), 2 (warning), 3 (error).
  name: state
  type: integer
- description: The number of source rows that failed.
  name: failedSourceRows
  type: integer
- description: The number of source rows processed successfully.
  name: successSourceRows
  type: integer
- description: The number of target rows that failed.
  name: failedTargetRows
  type: integer
- description: The number of target rows written successfully.
  name: successTargetRows
  type: integer
- description: The total number of rows processed successfully.
  name: totalSuccessRows
  type: integer
- description: The total number of rows that encountered errors.
  name: totalErrorRows
  type: integer
- description: The error message if the job failed.
  name: errorMsg
  type: string
- description: The user who started the job.
  name: startedBy
  type: string
- description: The context in which the job was run (e.g., API, SCHEDULER, UI).
  name: runContextType
  type: string
- description: Sub-entries for multi-step jobs.
  name: entries
  type: array
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-activity-log-entry-schema.json
slug: informatica-platform-rest-activity-log-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLogEntry\",\n  \"type\": \"object\",\n  \"description\": \"An entry in the activity log representing the execution status of a job.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The activity log entry ID.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of activity.\"\n    },\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the task or object.\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task or object.\"\n    },\n    \"runId\": {\n      \"type\": \"integer\",\n      \"description\": \"The job run ID.\"\n    },\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"The Secure Agent that ran the job.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The runtime environment used.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the job started.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the job completed.\"\n    },\n    \"state\": {\n      \"type\": \"integer\",\n      \"description\": \"The job execution state. Common values are 1 (success), 2 (warning), 3 (error).\"\n    },\n    \"failedSourceRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of source rows that failed.\"\n    },\n    \"successSourceRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of source rows processed successfully.\"\n    },\n    \"failedTargetRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of target rows that failed.\"\n    },\n    \"successTargetRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of target rows written successfully.\"\n    },\n    \"\
  totalSuccessRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of rows processed successfully.\"\n    },\n    \"totalErrorRows\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of rows that encountered errors.\"\n    },\n    \"errorMsg\": {\n      \"type\": \"string\",\n      \"description\": \"The error message if the job failed.\"\n    },\n    \"startedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who started the job.\"\n    },\n    \"runContextType\": {\n      \"type\": \"string\",\n      \"description\": \"The context in which the job was run (e.g., API, SCHEDULER, UI).\"\n    },\n    \"entries\": {\n      \"type\": \"array\",\n      \"description\": \"Sub-entries for multi-step jobs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-activity-log-entry-schema.json
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
title: ActivityLogEntry
---
