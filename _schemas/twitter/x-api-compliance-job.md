---
description: ComplianceJob schema from X API v2
layout: schema
name: ComplianceJob
properties_list:
- description: Creation time of the compliance job.
  name: created_at
  type: string
- description: Expiration time of the download URL.
  name: download_expires_at
  type: string
- description: URL from which the user will retrieve their compliance results.
  name: download_url
  type: string
- description: Compliance Job ID.
  name: id
  type: string
- description: User-provided name for a compliance job.
  name: name
  type: string
- description: Status of a compliance job.
  name: status
  type: string
- description: Type of compliance job to list.
  name: type
  type: string
- description: Expiration time of the upload URL.
  name: upload_expires_at
  type: string
- description: URL to which the user will upload their Tweet or user IDs.
  name: upload_url
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-compliance-job-schema.json
slug: x-api-compliance-job
source_filename: x-api-compliance-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-compliance-job-schema.json\",\n  \"title\": \"ComplianceJob\",\n  \"description\": \"ComplianceJob schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Creation time of the compliance job.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-01-06T18:40:40.000Z\"\n    },\n    \"download_expires_at\": {\n      \"type\": \"string\",\n      \"description\": \"Expiration time of the download URL.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-01-06T18:40:40.000Z\"\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL from which the user will retrieve their compliance results.\",\n      \"format\": \"uri\"\n    },\n    \"id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Compliance Job ID.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1372966999991541762\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided name for a compliance job.\",\n      \"maxLength\": 64,\n      \"example\": \"my-job\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of a compliance job.\",\n      \"enum\": [\n        \"created\",\n        \"in_progress\",\n        \"failed\",\n        \"complete\",\n        \"expired\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of compliance job to list.\",\n      \"enum\": [\n        \"tweets\",\n        \"users\"\n      ]\n    },\n    \"upload_expires_at\": {\n      \"type\": \"string\",\n      \"description\": \"Expiration time of the upload URL.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-01-06T18:40:40.000Z\"\n    },\n    \"upload_url\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"URL to which the user will upload their Tweet or user IDs.\",\n      \"format\": \"uri\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"created_at\",\n    \"upload_url\",\n    \"download_url\",\n    \"upload_expires_at\",\n    \"download_expires_at\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-compliance-job-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: ComplianceJob
---
