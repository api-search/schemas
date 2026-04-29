---
description: ''
layout: schema
name: BatchJobExecution
properties_list:
- description: ''
  name: executionId
  type: integer
- description: ''
  name: jobInstanceId
  type: integer
- description: ''
  name: jobName
  type: string
- description: ''
  name: batchStatus
  type: string
- description: ''
  name: exitStatus
  type: string
- description: ''
  name: createTime
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: lastUpdatedTime
  type: string
- description: ''
  name: jobParameters
  type: object
- description: ''
  name: stepExecutions
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/open-libertys-batch-job-execution-schema.json
slug: open-libertys-batch-job-execution
source_filename: open-libertys-batch-job-execution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchJobExecution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionId\": {\n      \"type\": \"integer\"\n    },\n    \"jobInstanceId\": {\n      \"type\": \"integer\"\n    },\n    \"jobName\": {\n      \"type\": \"string\"\n    },\n    \"batchStatus\": {\n      \"type\": \"string\"\n    },\n    \"exitStatus\": {\n      \"type\": \"string\"\n    },\n    \"createTime\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedTime\": {\n      \"type\": \"string\"\n    },\n    \"jobParameters\": {\n      \"type\": \"object\"\n    },\n    \"stepExecutions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/open-libertys-batch-job-execution-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: BatchJobExecution
---
