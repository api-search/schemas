---
description: The details of a task definition which describes the container and volume definitions of an Amazon ECS task.
layout: schema
name: TaskDefinition
properties_list:
- description: The full ARN of the task definition.
  name: taskDefinitionArn
  type: string
- description: ''
  name: containerDefinitions
  type: array
- description: The family of your task definition.
  name: family
  type: string
- description: ''
  name: taskRoleArn
  type: string
- description: ''
  name: executionRoleArn
  type: string
- description: ''
  name: networkMode
  type: string
- description: The revision of the task in a particular family.
  name: revision
  type: integer
- description: ''
  name: volumes
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: requiresAttributes
  type: array
- description: ''
  name: placementConstraints
  type: array
- description: ''
  name: compatibilities
  type: array
- description: ''
  name: requiresCompatibilities
  type: array
- description: ''
  name: cpu
  type: string
- description: ''
  name: memory
  type: string
- description: ''
  name: pidMode
  type: string
- description: ''
  name: ipcMode
  type: string
- description: ''
  name: inferenceAccelerators
  type: array
- description: Unix timestamp for when the task definition was registered.
  name: registeredAt
  type: number
- description: Unix timestamp for when the task definition was deregistered.
  name: deregisteredAt
  type: number
- description: ''
  name: registeredBy
  type: string
- description: ''
  name: enableFaultInjection
  type: boolean
- description: ''
  name: tags
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-task-definition-schema.json
slug: amazon-ecs-task-definition
source_filename: amazon-ecs-task-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskDefinition\",\n  \"type\": \"object\",\n  \"description\": \"The details of a task definition which describes the container and volume definitions of an Amazon ECS task.\",\n  \"properties\": {\n    \"taskDefinitionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The full ARN of the task definition.\"\n    },\n    \"containerDefinitions\": {\n      \"type\": \"array\"\n    },\n    \"family\": {\n      \"type\": \"string\",\n      \"description\": \"The family of your task definition.\"\n    },\n    \"taskRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"executionRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"networkMode\": {\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"type\": \"integer\",\n      \"description\": \"The revision of the task in a particular family.\"\n    },\n    \"volumes\": {\n      \"type\": \"array\"\n    },\n    \"status\"\
  : {\n      \"type\": \"string\"\n    },\n    \"requiresAttributes\": {\n      \"type\": \"array\"\n    },\n    \"placementConstraints\": {\n      \"type\": \"array\"\n    },\n    \"compatibilities\": {\n      \"type\": \"array\"\n    },\n    \"requiresCompatibilities\": {\n      \"type\": \"array\"\n    },\n    \"cpu\": {\n      \"type\": \"string\"\n    },\n    \"memory\": {\n      \"type\": \"string\"\n    },\n    \"pidMode\": {\n      \"type\": \"string\"\n    },\n    \"ipcMode\": {\n      \"type\": \"string\"\n    },\n    \"inferenceAccelerators\": {\n      \"type\": \"array\"\n    },\n    \"registeredAt\": {\n      \"type\": \"number\",\n      \"description\": \"Unix timestamp for when the task definition was registered.\"\n    },\n    \"deregisteredAt\": {\n      \"type\": \"number\",\n      \"description\": \"Unix timestamp for when the task definition was deregistered.\"\n    },\n    \"registeredBy\": {\n      \"type\": \"string\"\n    },\n    \"enableFaultInjection\": {\n    \
  \  \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-task-definition-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: TaskDefinition
---
