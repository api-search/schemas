---
description: Request body for creating a DataSync task.
layout: schema
name: Create Task Request
properties_list:
- description: ''
  name: SourceLocationArn
  type: string
- description: ''
  name: DestinationLocationArn
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: CloudWatchLogGroupArn
  type: string
- description: ''
  name: Options
  type: object
- description: ''
  name: Tags
  type: array
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/create-task-request-schema.json
slug: create-task-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/create-task-request-schema.json\",\n  \"title\": \"Create Task Request\",\n  \"description\": \"Request body for creating a DataSync task.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"SourceLocationArn\",\n    \"DestinationLocationArn\"\n  ],\n  \"properties\": {\n    \"SourceLocationArn\": {\n      \"type\": \"string\"\n    },\n    \"DestinationLocationArn\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"CloudWatchLogGroupArn\": {\n      \"type\": \"string\"\n    },\n    \"Options\": {\n      \"type\": \"object\"\n    },\n    \"Tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/create-task-request-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Create Task Request
---
