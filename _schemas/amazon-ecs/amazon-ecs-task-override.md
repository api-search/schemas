---
description: The overrides associated with a task.
layout: schema
name: TaskOverride
properties_list:
- description: ''
  name: containerOverrides
  type: array
- description: ''
  name: cpu
  type: string
- description: ''
  name: memory
  type: string
- description: ''
  name: taskRoleArn
  type: string
- description: ''
  name: executionRoleArn
  type: string
- description: ''
  name: inferenceAcceleratorOverrides
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-task-override-schema.json
slug: amazon-ecs-task-override
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskOverride\",\n  \"type\": \"object\",\n  \"description\": \"The overrides associated with a task.\",\n  \"properties\": {\n    \"containerOverrides\": {\n      \"type\": \"array\"\n    },\n    \"cpu\": {\n      \"type\": \"string\"\n    },\n    \"memory\": {\n      \"type\": \"string\"\n    },\n    \"taskRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"executionRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"inferenceAcceleratorOverrides\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-task-override-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: TaskOverride
---
