---
description: A summary of a DataSync task.
layout: schema
name: Task List Entry
properties_list:
- description: ''
  name: TaskArn
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Status
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/task-list-entry-schema.json
slug: task-list-entry
source_filename: task-list-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/task-list-entry-schema.json\",\n  \"title\": \"Task List Entry\",\n  \"description\": \"A summary of a DataSync task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskArn\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/task-list-entry-schema.json
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Task List Entry
---
