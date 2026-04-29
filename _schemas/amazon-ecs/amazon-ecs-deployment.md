---
description: ''
layout: schema
name: Deployment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: taskDefinition
  type: string
- description: ''
  name: desiredCount
  type: integer
- description: ''
  name: pendingCount
  type: integer
- description: ''
  name: runningCount
  type: integer
- description: ''
  name: failedTasks
  type: integer
- description: ''
  name: createdAt
  type: number
- description: ''
  name: updatedAt
  type: number
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
  name: rolloutState
  type: string
- description: ''
  name: rolloutStateReason
  type: string
- description: ''
  name: capacityProviderStrategy
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-deployment-schema.json
slug: amazon-ecs-deployment
source_filename: amazon-ecs-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"taskDefinition\": {\n      \"type\": \"string\"\n    },\n    \"desiredCount\": {\n      \"type\": \"integer\"\n    },\n    \"pendingCount\": {\n      \"type\": \"integer\"\n    },\n    \"runningCount\": {\n      \"type\": \"integer\"\n    },\n    \"failedTasks\": {\n      \"type\": \"integer\"\n    },\n    \"createdAt\": {\n      \"type\": \"number\"\n    },\n    \"updatedAt\": {\n      \"type\": \"number\"\n    },\n    \"launchType\": {\n      \"type\": \"string\"\n    },\n    \"platformVersion\": {\n      \"type\": \"string\"\n    },\n    \"platformFamily\": {\n      \"type\": \"string\"\n    },\n    \"rolloutState\": {\n      \"type\": \"string\"\n    },\n    \"rolloutStateReason\": {\n      \"type\": \"string\"\n    },\n\
  \    \"capacityProviderStrategy\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-deployment-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Deployment
---
