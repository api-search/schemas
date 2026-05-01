---
description: Represents a Dapr scheduled job, including its schedule expression, due time, repeat count, time-to-live, and data payload for triggered execution.
layout: schema
name: Dapr Job
properties_list:
- description: The name of the job.
  name: name
  type: string
- description: The schedule for the job using a cron expression or duration (e.g., @every 5s).
  name: schedule
  type: string
- description: The time at which the job should be triggered (RFC 3339 or duration format).
  name: dueTime
  type: string
- description: The number of times the job should be triggered.
  name: repeats
  type: integer
- description: Time-to-live for the job.
  name: ttl
  type: string
- description: The data payload to include with the job trigger.
  name: data
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/job.json
slug: job
source_filename: job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/job.json\",\n  \"title\": \"Dapr Job\",\n  \"description\": \"Represents a Dapr scheduled job, including its schedule expression, due time, repeat count, time-to-live, and data payload for triggered execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job.\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"The schedule for the job using a cron expression or duration (e.g., @every 5s).\"\n    },\n    \"dueTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time at which the job should be triggered (RFC 3339 or duration format).\"\n    },\n    \"repeats\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times the job should be triggered.\"\n    },\n    \"ttl\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Time-to-live for the job.\"\n    },\n    \"data\": {\n      \"description\": \"The data payload to include with the job trigger.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/job.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Job
---
