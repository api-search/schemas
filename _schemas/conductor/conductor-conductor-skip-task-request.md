---
description: ''
layout: schema
name: SkipTaskRequest
properties_list:
- description: Input for the skipped task
  name: taskInput
  type: object
- description: Output to set for the skipped task
  name: taskOutput
  type: object
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-skip-task-request-schema.json
slug: conductor-conductor-skip-task-request
source_filename: conductor-conductor-skip-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SkipTaskRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input for the skipped task\"\n    },\n    \"taskOutput\": {\n      \"type\": \"object\",\n      \"description\": \"Output to set for the skipped task\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-skip-task-request-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: SkipTaskRequest
---
