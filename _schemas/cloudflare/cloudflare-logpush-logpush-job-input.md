---
description: ''
layout: schema
name: LogpushJobInput
properties_list:
- description: Name for the job.
  name: name
  type: string
- description: Whether the job is active.
  name: enabled
  type: boolean
- description: The log dataset to push.
  name: dataset
  type: string
- description: Destination URI.
  name: destination_conf
  type: string
- description: Options for log fields and formatting.
  name: logpull_options
  type: string
- description: ''
  name: frequency
  type: string
- description: JSON filter expression to limit logs pushed.
  name: filter
  type: string
- description: The ownership challenge token.
  name: ownership_challenge
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-logpush-logpush-job-input-schema.json
slug: cloudflare-logpush-logpush-job-input
source_filename: cloudflare-logpush-logpush-job-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogpushJobInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the job.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job is active.\"\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The log dataset to push.\"\n    },\n    \"destination_conf\": {\n      \"type\": \"string\",\n      \"description\": \"Destination URI.\"\n    },\n    \"logpull_options\": {\n      \"type\": \"string\",\n      \"description\": \"Options for log fields and formatting.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"JSON filter expression to limit logs pushed.\"\n    },\n    \"ownership_challenge\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The ownership challenge token.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-logpush-logpush-job-input-schema.json
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
title: LogpushJobInput
---
