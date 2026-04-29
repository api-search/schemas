---
description: A job posting from a connected ATS system.
layout: schema
name: Job
properties_list:
- description: Job ID.
  name: id
  type: string
- description: Job title.
  name: title
  type: string
- description: Hiring department.
  name: department
  type: string
- description: Job location or remote.
  name: location
  type: string
- description: Job posting status.
  name: status
  type: string
- description: Job creation timestamp.
  name: created_at
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-job-schema.json
slug: bindbee-job
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"description\": \"A job posting from a connected ATS system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID.\",\n      \"example\": \"job-abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title.\",\n      \"example\": \"Senior Software Engineer\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Hiring department.\",\n      \"example\": \"Engineering\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Job location or remote.\",\n      \"example\": \"Remote\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Job posting status.\",\n      \"enum\": [\n        \"open\",\n        \"closed\",\n        \"draft\"\n      ],\n      \"example\": \"open\"\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job creation timestamp.\",\n      \"example\": \"2024-04-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-job-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Job
---
