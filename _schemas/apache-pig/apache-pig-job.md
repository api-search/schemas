---
description: Job schema from Apache Pig
layout: schema
name: Job
properties_list:
- description: ''
  name: jobId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: submittedAt
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: completedAt
  type: string
- description: ''
  name: executionEngine
  type: string
- description: Progress percentage 0-100
  name: progress
  type: number
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-job-schema.json
slug: apache-pig-job
source_filename: apache-pig-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Job schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"example\": \"job_20260419_001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"sales-analysis\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"submitted\",\n        \"running\",\n        \"succeeded\",\n        \"failed\",\n        \"killed\"\n      ],\n      \"example\": \"running\"\n    },\n    \"submittedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T10:01:00Z\"\
  \n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"executionEngine\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"mapreduce\",\n        \"tez\",\n        \"local\"\n      ],\n      \"example\": \"tez\"\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"description\": \"Progress percentage 0-100\",\n      \"example\": 45.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: Job
---
