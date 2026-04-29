---
description: A monitored data pipeline job execution
layout: schema
name: PipelineJob
properties_list:
- description: Job execution identifier
  name: id
  type: string
- description: Pipeline job name
  name: name
  type: string
- description: Platform running the job
  name: platform
  type: string
- description: Job execution status
  name: status
  type: string
- description: Job start time
  name: startTime
  type: string
- description: Job end time
  name: endTime
  type: string
- description: Job duration in seconds
  name: durationSeconds
  type: integer
- description: SLA compliance status
  name: slaStatus
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-pipeline-job-schema.json
slug: adoc-api-pipeline-job
source_filename: adoc-api-pipeline-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/pipeline-job.json\",\n  \"title\": \"PipelineJob\",\n  \"type\": \"object\",\n  \"description\": \"A monitored data pipeline job execution\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job execution identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline job name\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Platform running the job\",\n      \"enum\": [\n        \"databricks\",\n        \"airflow\",\n        \"glue\",\n        \"dataflow\",\n        \"spark\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Job execution status\",\n      \"enum\": [\n        \"running\",\n        \"succeeded\",\n        \"failed\",\n        \"pending\"\n      ]\n    },\n    \"startTime\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job start time\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job end time\"\n    },\n    \"durationSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Job duration in seconds\"\n    },\n    \"slaStatus\": {\n      \"type\": \"string\",\n      \"description\": \"SLA compliance status\",\n      \"enum\": [\n        \"met\",\n        \"violated\",\n        \"at_risk\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-pipeline-job-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: PipelineJob
---
