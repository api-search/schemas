---
description: ''
layout: schema
name: RunTaskResponse
properties_list:
- description: ''
  name: tasks
  type: array
- description: ''
  name: failures
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-run-task-response-schema.json
slug: amazon-ecs-run-task-response
source_filename: amazon-ecs-run-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunTaskResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"type\": \"array\"\n    },\n    \"failures\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-run-task-response-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: RunTaskResponse
---
