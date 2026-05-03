---
description: A job executes a function at a set time, interval, or CRON schedule for automated recurring tasks.
layout: schema
name: PolyAPI Job
properties_list:
- description: The unique identifier of the job.
  name: id
  type: string
- description: The name of the job.
  name: name
  type: string
- description: A description of the job.
  name: description
  type: string
- description: The ID of the function to execute.
  name: functionId
  type: string
- description: The type of function to execute.
  name: functionType
  type: string
- description: The CRON expression or interval defining when the job runs.
  name: schedule
  type: string
- description: The state of the job.
  name: state
  type: string
- description: Timestamp of the last execution.
  name: lastRunAt
  type: string
- description: Timestamp of the next scheduled execution.
  name: nextRunAt
  type: string
- description: Timestamp when the job was created.
  name: createdAt
  type: string
- description: Timestamp when the job was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/job.json
slug: job
source_filename: job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/job.json\",\n  \"title\": \"PolyAPI Job\",\n  \"description\": \"A job executes a function at a set time, interval, or CRON schedule for automated recurring tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the job.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the job.\"\n    },\n    \"functionId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the function to execute.\"\n    },\n    \"functionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"server\", \"api\"],\n      \"description\": \"The type of function to execute.\"\n    },\n    \"schedule\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The CRON expression or interval defining when the job runs.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\"],\n      \"description\": \"The state of the job.\"\n    },\n    \"lastRunAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last execution.\"\n    },\n    \"nextRunAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the next scheduled execution.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"functionId\", \"functionType\", \"schedule\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/job.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Job
---
