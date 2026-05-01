---
description: A DataSync task defining source location, destination location, and transfer configuration.
layout: schema
name: Task
properties_list:
- description: The ARN of the DataSync task. This ARN uniquely identifies the task.
  name: TaskArn
  type: string
- description: The name of the task
  name: Name
  type: string
- description: ''
  name: Status
  type: string
- description: The ARN of the source location. This ARN uniquely identifies the location.
  name: SourceLocationArn
  type: string
- description: The ARN of the destination location. This ARN uniquely identifies the location.
  name: DestinationLocationArn
  type: string
- description: ''
  name: CurrentTaskExecutionArn
  type: string
- description: ''
  name: CloudWatchLogGroupArn
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/task-schema.json
slug: task
source_filename: task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"A DataSync task defining source location, destination location, and transfer configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the DataSync task. This ARN uniquely identifies the task.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"CREATING\",\n        \"QUEUED\",\n        \"RUNNING\",\n        \"UNAVAILABLE\"\n      ]\n    },\n    \"SourceLocationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the source location. This ARN uniquely identifies the location.\"\n    },\n    \"DestinationLocationArn\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the destination location. This ARN uniquely identifies the location.\"\n    },\n    \"CurrentTaskExecutionArn\": {\n      \"type\": \"string\"\n    },\n    \"CloudWatchLogGroupArn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/task-schema.json
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Task
---
