---
description: JobLogs schema from Apache Pig
layout: schema
name: JobLogs
properties_list:
- description: ''
  name: jobId
  type: string
- description: ''
  name: logs
  type: array
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-job-logs-schema.json
slug: apache-pig-job-logs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-logs-schema.json\",\n  \"title\": \"JobLogs\",\n  \"description\": \"JobLogs schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"example\": \"job_20260419_001\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"2026-04-19 10:00:00 INFO Pig script started\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-job-logs-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: JobLogs
---
