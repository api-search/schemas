---
description: Provides details of a single job.
layout: schema
name: JobResponse
properties_list:
- description: ''
  name: jobId
  type: integer
- description: ''
  name: status
  type: object
- description: ''
  name: jobType
  type: object
- description: ''
  name: startTime
  type: string
- description: ''
  name: connectionId
  type: string
- description: ''
  name: lastUpdatedAt
  type: string
- description: Duration of a sync in ISO_8601 format
  name: duration
  type: string
- description: ''
  name: bytesSynced
  type: integer
- description: ''
  name: rowsSynced
  type: integer
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-job-response-schema.json
slug: airbyte-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-response-schema.json\",\n  \"title\": \"JobResponse\",\n  \"description\": \"Provides details of a single job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/JobStatusEnum\"\n    },\n    \"jobType\": {\n      \"$ref\": \"#/components/schemas/JobTypeEnum\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"connectionId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"description\": \"Duration of a sync in ISO_8601 format\",\n      \"type\": \"string\"\n    },\n    \"bytesSynced\": {\n      \"format\": \"int64\",\n      \"type\"\
  : \"integer\"\n    },\n    \"rowsSynced\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"status\",\n    \"jobType\",\n    \"startTime\",\n    \"connectionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: JobResponse
---
