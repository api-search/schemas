---
description: Response after creating a DataSync task.
layout: schema
name: Create Task Response
properties_list:
- description: The ARN of the newly created task
  name: TaskArn
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/create-task-response-schema.json
slug: create-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/create-task-response-schema.json\",\n  \"title\": \"Create Task Response\",\n  \"description\": \"Response after creating a DataSync task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the newly created task\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/create-task-response-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Create Task Response
---
