---
description: Job status response
layout: schema
name: JobStatus
properties_list:
- description: ''
  name: jobName
  type: string
- description: ''
  name: jobId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-job-status-schema.json
slug: apache-samza-job-status
source_filename: apache-samza-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"Job status response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobName\": {\n      \"type\": \"string\"\n    },\n    \"jobId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STARTED\",\n        \"STOPPED\",\n        \"NEW\",\n        \"STARTING\",\n        \"STOPPING\",\n        \"RESTARTING\",\n        \"UNKNOWN\"\n      ]\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-status-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: JobStatus
---
