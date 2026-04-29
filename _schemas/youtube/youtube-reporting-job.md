---
description: ''
layout: schema
name: Job
properties_list:
- description: The server-generated ID of the job.
  name: id
  type: string
- description: The type of reports that the job creates.
  name: reportTypeId
  type: string
- description: The name of the job. Max length is 100 characters.
  name: name
  type: string
- description: The date and time when the job was created.
  name: createTime
  type: string
- description: The date and time when the job will expire.
  name: expireTime
  type: string
- description: Whether the job is system-managed.
  name: systemManaged
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-reporting-job-schema.json
slug: youtube-reporting-job
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The server-generated ID of the job.\",\n      \"example\": \"abc123def456\"\n    },\n    \"reportTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"The type of reports that the job creates.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job. Max length is 100 characters.\",\n      \"example\": \"Example Title\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the job was created.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"expireTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the job will expire.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"systemManaged\": {\n\
  \      \"type\": \"boolean\",\n      \"description\": \"Whether the job is system-managed.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-reporting-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-reporting-job-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Job
---
