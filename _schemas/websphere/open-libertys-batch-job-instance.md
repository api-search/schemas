---
description: ''
layout: schema
name: BatchJobInstance
properties_list:
- description: ''
  name: jobInstanceId
  type: integer
- description: ''
  name: jobName
  type: string
- description: ''
  name: appName
  type: string
- description: ''
  name: submitter
  type: string
- description: ''
  name: batchStatus
  type: string
- description: ''
  name: createTime
  type: string
- description: ''
  name: lastUpdatedTime
  type: string
- description: ''
  name: jobParameters
  type: object
- description: ''
  name: _links
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/open-libertys-batch-job-instance-schema.json
slug: open-libertys-batch-job-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchJobInstance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobInstanceId\": {\n      \"type\": \"integer\"\n    },\n    \"jobName\": {\n      \"type\": \"string\"\n    },\n    \"appName\": {\n      \"type\": \"string\"\n    },\n    \"submitter\": {\n      \"type\": \"string\"\n    },\n    \"batchStatus\": {\n      \"type\": \"string\"\n    },\n    \"createTime\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedTime\": {\n      \"type\": \"string\"\n    },\n    \"jobParameters\": {\n      \"type\": \"object\"\n    },\n    \"_links\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/open-libertys-batch-job-instance-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: BatchJobInstance
---
