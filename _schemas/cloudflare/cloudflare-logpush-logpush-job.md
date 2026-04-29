---
description: ''
layout: schema
name: LogpushJob
properties_list:
- description: The unique identifier of the job.
  name: id
  type: integer
- description: A human-readable name for the job.
  name: name
  type: string
- description: Whether the job is active.
  name: enabled
  type: boolean
- description: The log dataset.
  name: dataset
  type: string
- description: The destination configuration URI.
  name: destination_conf
  type: string
- description: Logpull options specifying fields, timestamps, and sample rate.
  name: logpull_options
  type: string
- description: Log push frequency.
  name: frequency
  type: string
- description: Timestamp of the last successful push.
  name: last_complete
  type: string
- description: Timestamp of the last error.
  name: last_error
  type: string
- description: Last error message.
  name: error_message
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-logpush-logpush-job-schema.json
slug: cloudflare-logpush-logpush-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogpushJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the job.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the job.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job is active.\"\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The log dataset.\"\n    },\n    \"destination_conf\": {\n      \"type\": \"string\",\n      \"description\": \"The destination configuration URI.\"\n    },\n    \"logpull_options\": {\n      \"type\": \"string\",\n      \"description\": \"Logpull options specifying fields, timestamps, and sample rate.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Log push frequency.\"\n    },\n  \
  \  \"last_complete\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last successful push.\"\n    },\n    \"last_error\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last error.\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Last error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-logpush-logpush-job-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: LogpushJob
---
