---
description: JobStatus schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: JobStatus
properties_list:
- description: Unique job identifier.
  name: id
  type: string
- description: Type of asynchronous job.
  name: type
  type: string
- description: Current status of the job.
  name: status
  type: string
- description: Final result of the job once completed.
  name: result
  type: string
- description: Timestamp when the job started.
  name: start_ts
  type: string
- description: Timestamp when the job completed.
  name: end_ts
  type: string
- description: Job description.
  name: description
  type: string
- description: Job status detail messages.
  name: details
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-job-status-schema.json
slug: prisma-access-api-job-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobStatus\",\n  \"description\": \"JobStatus schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-job-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique job identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of asynchronous job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current status of the job.\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OK\",\n        \"FAIL\"\n      ],\n      \"description\": \"Final result of\
  \ the job once completed.\"\n    },\n    \"start_ts\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job started.\"\n    },\n    \"end_ts\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job completed.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Job description.\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Job status detail messages.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-job-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: JobStatus
---
