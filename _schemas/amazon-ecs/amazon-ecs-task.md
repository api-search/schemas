---
description: Details on a task in a cluster.
layout: schema
name: Task
properties_list:
- description: The ARN of the task.
  name: taskArn
  type: string
- description: The ARN of the cluster that hosts the task.
  name: clusterArn
  type: string
- description: The ARN of the task definition that creates the task.
  name: taskDefinitionArn
  type: string
- description: The ARN of the container instances that host the task.
  name: containerInstanceArn
  type: string
- description: The last known status for the task.
  name: lastStatus
  type: string
- description: The desired status of the task.
  name: desiredStatus
  type: string
- description: ''
  name: cpu
  type: string
- description: ''
  name: memory
  type: string
- description: ''
  name: containers
  type: array
- description: ''
  name: startedBy
  type: string
- description: ''
  name: version
  type: integer
- description: ''
  name: stoppedReason
  type: string
- description: ''
  name: stopCode
  type: string
- description: ''
  name: connectivity
  type: string
- description: ''
  name: connectivityAt
  type: number
- description: ''
  name: pullStartedAt
  type: number
- description: ''
  name: pullStoppedAt
  type: number
- description: ''
  name: executionStoppedAt
  type: number
- description: ''
  name: createdAt
  type: number
- description: ''
  name: startedAt
  type: number
- description: ''
  name: stoppingAt
  type: number
- description: ''
  name: stoppedAt
  type: number
- description: ''
  name: group
  type: string
- description: ''
  name: launchType
  type: string
- description: ''
  name: platformVersion
  type: string
- description: ''
  name: platformFamily
  type: string
- description: ''
  name: capacityProviderName
  type: string
- description: ''
  name: availabilityZone
  type: string
- description: ''
  name: attachments
  type: array
- description: ''
  name: healthStatus
  type: string
- description: ''
  name: enableExecuteCommand
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: inferenceAccelerators
  type: array
- description: ''
  name: attributes
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-task-schema.json
slug: amazon-ecs-task
source_filename: amazon-ecs-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Task\",\n  \"type\": \"object\",\n  \"description\": \"Details on a task in a cluster.\",\n  \"properties\": {\n    \"taskArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the task.\"\n    },\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the cluster that hosts the task.\"\n    },\n    \"taskDefinitionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the task definition that creates the task.\"\n    },\n    \"containerInstanceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the container instances that host the task.\"\n    },\n    \"lastStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The last known status for the task.\"\n    },\n    \"desiredStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The desired status of the task.\"\n    },\n    \"\
  cpu\": {\n      \"type\": \"string\"\n    },\n    \"memory\": {\n      \"type\": \"string\"\n    },\n    \"containers\": {\n      \"type\": \"array\"\n    },\n    \"startedBy\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"integer\"\n    },\n    \"stoppedReason\": {\n      \"type\": \"string\"\n    },\n    \"stopCode\": {\n      \"type\": \"string\"\n    },\n    \"connectivity\": {\n      \"type\": \"string\"\n    },\n    \"connectivityAt\": {\n      \"type\": \"number\"\n    },\n    \"pullStartedAt\": {\n      \"type\": \"number\"\n    },\n    \"pullStoppedAt\": {\n      \"type\": \"number\"\n    },\n    \"executionStoppedAt\": {\n      \"type\": \"number\"\n    },\n    \"createdAt\": {\n      \"type\": \"number\"\n    },\n    \"startedAt\": {\n      \"type\": \"number\"\n    },\n    \"stoppingAt\": {\n      \"type\": \"number\"\n    },\n    \"stoppedAt\": {\n      \"type\": \"number\"\n    },\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"\
  launchType\": {\n      \"type\": \"string\"\n    },\n    \"platformVersion\": {\n      \"type\": \"string\"\n    },\n    \"platformFamily\": {\n      \"type\": \"string\"\n    },\n    \"capacityProviderName\": {\n      \"type\": \"string\"\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\"\n    },\n    \"attachments\": {\n      \"type\": \"array\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\"\n    },\n    \"enableExecuteCommand\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"inferenceAccelerators\": {\n      \"type\": \"array\"\n    },\n    \"attributes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-task-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Task
---
