---
description: Summary representation of an execution job
layout: schema
name: JobSummary
properties_list:
- description: Unique job identifier
  name: id
  type: string
- description: Date the job was created
  name: createDate
  type: string
- description: Current job status
  name: status
  type: string
- description: Job priority
  name: priority
  type: string
- description: Worker tag for execution routing
  name: workerTag
  type: string
- description: Whether the job runs with AMP engine
  name: runWithE2
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-job-summary-schema.json
slug: alteryx-server-v3-job-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary representation of an execution job\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique job identifier\"\n    },\n    \"createDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the job was created\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current job status\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Job priority\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Worker tag for execution routing\"\n    },\n    \"runWithE2\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job runs with AMP engine\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-job-summary-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: JobSummary
---
