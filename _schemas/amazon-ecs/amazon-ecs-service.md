---
description: Details on a service within a cluster. A service runs and maintains a specified number of instances of a task definition.
layout: schema
name: Service
properties_list:
- description: The ARN that identifies the service.
  name: serviceArn
  type: string
- description: The name of your service.
  name: serviceName
  type: string
- description: The ARN of the cluster that hosts the service.
  name: clusterArn
  type: string
- description: ''
  name: loadBalancers
  type: array
- description: ''
  name: serviceRegistries
  type: array
- description: The status of the service.
  name: status
  type: string
- description: The desired number of instantiations of the task definition to keep running on the service.
  name: desiredCount
  type: integer
- description: The number of tasks in the cluster that are in the RUNNING state.
  name: runningCount
  type: integer
- description: The number of tasks in the cluster that are in the PENDING state.
  name: pendingCount
  type: integer
- description: ''
  name: launchType
  type: string
- description: ''
  name: capacityProviderStrategy
  type: array
- description: ''
  name: platformVersion
  type: string
- description: ''
  name: platformFamily
  type: string
- description: The task definition ARN used by tasks in the service.
  name: taskDefinition
  type: string
- description: ''
  name: deployments
  type: array
- description: ''
  name: roleArn
  type: string
- description: ''
  name: events
  type: array
- description: The Unix timestamp for when the service was created.
  name: createdAt
  type: number
- description: ''
  name: placementConstraints
  type: array
- description: ''
  name: placementStrategy
  type: array
- description: ''
  name: healthCheckGracePeriodSeconds
  type: integer
- description: ''
  name: schedulingStrategy
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: createdBy
  type: string
- description: ''
  name: enableECSManagedTags
  type: boolean
- description: ''
  name: enableExecuteCommand
  type: boolean
- description: ''
  name: propagateTags
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-service-schema.json
slug: amazon-ecs-service
source_filename: amazon-ecs-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"type\": \"object\",\n  \"description\": \"Details on a service within a cluster. A service runs and maintains a specified number of instances of a task definition.\",\n  \"properties\": {\n    \"serviceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN that identifies the service.\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of your service.\"\n    },\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the cluster that hosts the service.\"\n    },\n    \"loadBalancers\": {\n      \"type\": \"array\"\n    },\n    \"serviceRegistries\": {\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the service.\"\n    },\n    \"desiredCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The desired\
  \ number of instantiations of the task definition to keep running on the service.\"\n    },\n    \"runningCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks in the cluster that are in the RUNNING state.\"\n    },\n    \"pendingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks in the cluster that are in the PENDING state.\"\n    },\n    \"launchType\": {\n      \"type\": \"string\"\n    },\n    \"capacityProviderStrategy\": {\n      \"type\": \"array\"\n    },\n    \"platformVersion\": {\n      \"type\": \"string\"\n    },\n    \"platformFamily\": {\n      \"type\": \"string\"\n    },\n    \"taskDefinition\": {\n      \"type\": \"string\",\n      \"description\": \"The task definition ARN used by tasks in the service.\"\n    },\n    \"deployments\": {\n      \"type\": \"array\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\"\n    },\n    \"events\": {\n      \"type\": \"array\"\n    },\n    \"createdAt\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"The Unix timestamp for when the service was created.\"\n    },\n    \"placementConstraints\": {\n      \"type\": \"array\"\n    },\n    \"placementStrategy\": {\n      \"type\": \"array\"\n    },\n    \"healthCheckGracePeriodSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"schedulingStrategy\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"enableECSManagedTags\": {\n      \"type\": \"boolean\"\n    },\n    \"enableExecuteCommand\": {\n      \"type\": \"boolean\"\n    },\n    \"propagateTags\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-service-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Service
---
