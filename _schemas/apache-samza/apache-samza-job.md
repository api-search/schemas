---
description: Samza stream processing job
layout: schema
name: Job
properties_list:
- description: Job name
  name: jobName
  type: string
- description: Job identifier
  name: jobId
  type: string
- description: Current job status
  name: status
  type: string
- description: Number of containers running
  name: containersCount
  type: integer
- description: Total task count
  name: taskCount
  type: integer
provider_name: Apache Samza
provider_slug: apache-samza
schema_file: json-schema/apache-samza-job-schema.json
slug: apache-samza-job
source_filename: apache-samza-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Samza stream processing job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobName\": {\n      \"type\": \"string\",\n      \"description\": \"Job name\"\n    },\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STARTED\",\n        \"STOPPED\",\n        \"NEW\",\n        \"STARTING\",\n        \"STOPPING\",\n        \"RESTARTING\",\n        \"UNKNOWN\"\n      ],\n      \"description\": \"Current job status\"\n    },\n    \"containersCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of containers running\"\n    },\n    \"taskCount\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Total task count\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-samza/refs/heads/main/json-schema/apache-samza-job-schema.json
tags:
- Big Data
- Hadoop
- Kafka
- Stream Processing
- Streaming
- Apache
- Open Source
title: Job
---
