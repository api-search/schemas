---
description: An Amazon EC2 instance that is registered into an ECS cluster and running the ECS agent.
layout: schema
name: ContainerInstance
properties_list:
- description: ''
  name: containerInstanceArn
  type: string
- description: ''
  name: ec2InstanceId
  type: string
- description: ''
  name: version
  type: integer
- description: ''
  name: versionInfo
  type: object
- description: ''
  name: remainingResources
  type: array
- description: ''
  name: registeredResources
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: statusReason
  type: string
- description: ''
  name: agentConnected
  type: boolean
- description: ''
  name: runningTasksCount
  type: integer
- description: ''
  name: pendingTasksCount
  type: integer
- description: ''
  name: agentUpdateStatus
  type: string
- description: ''
  name: attributes
  type: array
- description: ''
  name: registeredAt
  type: number
- description: ''
  name: attachments
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: capacityProviderName
  type: string
- description: ''
  name: healthStatus
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-container-instance-schema.json
slug: amazon-ecs-container-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerInstance\",\n  \"type\": \"object\",\n  \"description\": \"An Amazon EC2 instance that is registered into an ECS cluster and running the ECS agent.\",\n  \"properties\": {\n    \"containerInstanceArn\": {\n      \"type\": \"string\"\n    },\n    \"ec2InstanceId\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"integer\"\n    },\n    \"versionInfo\": {\n      \"type\": \"object\"\n    },\n    \"remainingResources\": {\n      \"type\": \"array\"\n    },\n    \"registeredResources\": {\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"statusReason\": {\n      \"type\": \"string\"\n    },\n    \"agentConnected\": {\n      \"type\": \"boolean\"\n    },\n    \"runningTasksCount\": {\n      \"type\": \"integer\"\n    },\n    \"pendingTasksCount\": {\n      \"type\": \"integer\"\n    },\n    \"agentUpdateStatus\":\
  \ {\n      \"type\": \"string\"\n    },\n    \"attributes\": {\n      \"type\": \"array\"\n    },\n    \"registeredAt\": {\n      \"type\": \"number\"\n    },\n    \"attachments\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"capacityProviderName\": {\n      \"type\": \"string\"\n    },\n    \"healthStatus\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-container-instance-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ContainerInstance
---
