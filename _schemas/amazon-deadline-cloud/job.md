---
description: A rendering job submitted to a queue in Amazon Deadline Cloud.
layout: schema
name: Job
properties_list:
- description: The unique identifier of the job
  name: jobId
  type: string
- description: ''
  name: queueId
  type: string
- description: ''
  name: farmId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: lifecycleStatus
  type: string
- description: ''
  name: taskRunStatus
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: createdAt
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/job-schema.json
slug: job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A rendering job submitted to a queue in Amazon Deadline Cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the job\"\n    },\n    \"queueId\": {\n      \"type\": \"string\"\n    },\n    \"farmId\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleStatus\": {\n      \"type\": \"string\"\n    },\n    \"taskRunStatus\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/job-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: Job
---
