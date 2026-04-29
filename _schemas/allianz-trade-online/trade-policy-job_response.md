---
description: Async job status response
layout: schema
name: JobResponse
properties_list:
- description: Unique identifier for the async job
  name: jobId
  type: string
- description: Current status of the job
  name: status
  type: string
- description: Result data after successful job completion
  name: result
  type: object
- description: When the job was created
  name: createdAt
  type: string
- description: When the job completed (null if still pending)
  name: completedAt
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-policy-job_response-schema.json
slug: trade-policy-job_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-policy-job_response-schema.json\",\n  \"title\": \"JobResponse\",\n  \"type\": \"object\",\n  \"description\": \"Async job status response\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the async job\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the job\",\n      \"enum\": [\n        \"pending\",\n        \"processed\",\n        \"failed\"\n      ]\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"Result data after successful job completion\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the job was created\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"When the job completed (null if still pending)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-policy-job_response-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: JobResponse
---
