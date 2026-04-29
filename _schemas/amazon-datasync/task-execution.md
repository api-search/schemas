---
description: A specific execution run of a DataSync task.
layout: schema
name: Task Execution
properties_list:
- description: The ARN of the task execution. This ARN uniquely identifies the execution.
  name: TaskExecutionArn
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EstimatedFilesToTransfer
  type: integer
- description: ''
  name: FilesTransferred
  type: integer
- description: ''
  name: BytesTransferred
  type: integer
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/task-execution-schema.json
slug: task-execution
source_filename: task-execution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/task-execution-schema.json\",\n  \"title\": \"Task Execution\",\n  \"description\": \"A specific execution run of a DataSync task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskExecutionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the task execution. This ARN uniquely identifies the execution.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"QUEUED\",\n        \"LAUNCHING\",\n        \"PREPARING\",\n        \"TRANSFERRING\",\n        \"VERIFYING\",\n        \"SUCCESS\",\n        \"ERROR\"\n      ]\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EstimatedFilesToTransfer\": {\n      \"type\": \"integer\"\n    },\n    \"FilesTransferred\": {\n      \"type\": \"integer\"\n    },\n    \"BytesTransferred\"\
  : {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/task-execution-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Task Execution
---
