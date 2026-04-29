---
description: ''
layout: schema
name: RunTaskRequest
properties_list:
- description: The family and revision or full ARN of the task definition to run.
  name: taskDefinition
  type: string
- description: The short name or full ARN of the cluster to run the task on.
  name: cluster
  type: string
- description: The number of instantiations of the specified task to place on your cluster (1-10).
  name: count
  type: integer
- description: The launch type on which to run your task.
  name: launchType
  type: string
- description: ''
  name: capacityProviderStrategy
  type: array
- description: The platform version the task uses (Fargate launch type only).
  name: platformVersion
  type: string
- description: ''
  name: placementConstraints
  type: array
- description: ''
  name: placementStrategy
  type: array
- description: The name of the task group to associate with the task.
  name: group
  type: string
- description: An optional tag specified when a task is started.
  name: startedBy
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: enableECSManagedTags
  type: boolean
- description: Whether to enable Amazon ECS Exec for the task.
  name: enableExecuteCommand
  type: boolean
- description: ''
  name: propagateTags
  type: string
- description: An identifier you provide to ensure the idempotency of the request.
  name: clientToken
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-run-task-request-schema.json
slug: amazon-ecs-run-task-request
source_filename: amazon-ecs-run-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunTaskRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskDefinition\": {\n      \"type\": \"string\",\n      \"description\": \"The family and revision or full ARN of the task definition to run.\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"The short name or full ARN of the cluster to run the task on.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of instantiations of the specified task to place on your cluster (1-10).\"\n    },\n    \"launchType\": {\n      \"type\": \"string\",\n      \"description\": \"The launch type on which to run your task.\"\n    },\n    \"capacityProviderStrategy\": {\n      \"type\": \"array\"\n    },\n    \"platformVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The platform version the task uses (Fargate launch type only).\"\n    },\n    \"\
  placementConstraints\": {\n      \"type\": \"array\"\n    },\n    \"placementStrategy\": {\n      \"type\": \"array\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task group to associate with the task.\"\n    },\n    \"startedBy\": {\n      \"type\": \"string\",\n      \"description\": \"An optional tag specified when a task is started.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"enableECSManagedTags\": {\n      \"type\": \"boolean\"\n    },\n    \"enableExecuteCommand\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Amazon ECS Exec for the task.\"\n    },\n    \"propagateTags\": {\n      \"type\": \"string\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier you provide to ensure the idempotency of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-run-task-request-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: RunTaskRequest
---
