---
description: A container that is part of a task.
layout: schema
name: Container
properties_list:
- description: ''
  name: containerArn
  type: string
- description: ''
  name: taskArn
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: image
  type: string
- description: ''
  name: imageDigest
  type: string
- description: ''
  name: runtimeId
  type: string
- description: ''
  name: lastStatus
  type: string
- description: ''
  name: exitCode
  type: integer
- description: ''
  name: reason
  type: string
- description: ''
  name: healthStatus
  type: string
- description: ''
  name: cpu
  type: string
- description: ''
  name: memory
  type: string
- description: ''
  name: memoryReservation
  type: string
- description: ''
  name: gpuIds
  type: array
- description: ''
  name: networkBindings
  type: array
- description: ''
  name: networkInterfaces
  type: array
- description: ''
  name: managedAgents
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-container-schema.json
slug: amazon-ecs-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Container\",\n  \"type\": \"object\",\n  \"description\": \"A container that is part of a task.\",\n  \"properties\": {\n    \"containerArn\": {\n      \"type\": \"string\"\n    },\n    \"taskArn\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"image\": {\n      \"type\": \"string\"\n    },\n    \"imageDigest\": {\n      \"type\": \"string\"\n    },\n    \"runtimeId\": {\n      \"type\": \"string\"\n    },\n    \"lastStatus\": {\n      \"type\": \"string\"\n    },\n    \"exitCode\": {\n      \"type\": \"integer\"\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\"\n    },\n    \"cpu\": {\n      \"type\": \"string\"\n    },\n    \"memory\": {\n      \"type\": \"string\"\n    },\n    \"memoryReservation\": {\n      \"type\": \"string\"\n    },\n    \"gpuIds\": {\n      \"type\":\
  \ \"array\"\n    },\n    \"networkBindings\": {\n      \"type\": \"array\"\n    },\n    \"networkInterfaces\": {\n      \"type\": \"array\"\n    },\n    \"managedAgents\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-container-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Container
---
