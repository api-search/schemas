---
description: ''
layout: schema
name: Job
properties_list:
- description: The unique identifier for the job.
  name: id
  type: string
- description: The mode of the job.
  name: mode
  type: string
- description: The type of the job.
  name: type
  type: string
- description: The status code of the job. 0 = Active/Queued, 1 = Complete, 2 = Cancelled.
  name: status
  type: integer
- description: The progress of the job as a percentage.
  name: progress
  type: integer
- description: The date and time the job was created.
  name: createdAt
  type: string
- description: The date and time the job started running.
  name: startedAt
  type: string
- description: The date and time the job finished.
  name: endedAt
  type: string
- description: The completion code. 0 = success, 1 = error, 2 = cancelled.
  name: finishCode
  type: integer
- description: A description of what the job is doing.
  name: title
  type: string
- description: Additional detail about the job.
  name: subtitle
  type: string
- description: ''
  name: statusNotes
  type: object
- description: ''
  name: extractRefreshJob
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-job-schema.json
slug: tableau-rest-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the job.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode of the job.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the job.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The status code of the job. 0 = Active/Queued, 1 = Complete, 2 = Cancelled.\"\n    },\n    \"progress\": {\n      \"type\": \"integer\",\n      \"description\": \"The progress of the job as a percentage.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was created.\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job started running.\"\
  \n    },\n    \"endedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job finished.\"\n    },\n    \"finishCode\": {\n      \"type\": \"integer\",\n      \"description\": \"The completion code. 0 = success, 1 = error, 2 = cancelled.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the job is doing.\"\n    },\n    \"subtitle\": {\n      \"type\": \"string\",\n      \"description\": \"Additional detail about the job.\"\n    },\n    \"statusNotes\": {\n      \"type\": \"object\"\n    },\n    \"extractRefreshJob\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-job-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Job
---
