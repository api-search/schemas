---
description: An Amazon ECS task definition
layout: schema
name: TaskDefinition
properties_list:
- description: Full ARN of the task definition
  name: taskDefinitionArn
  type: string
- description: Family of the task definition
  name: family
  type: string
- description: Revision number
  name: revision
  type: integer
- description: Task definition status
  name: status
  type: string
- description: Launch types the task definition is compatible with
  name: requiresCompatibilities
  type: array
- description: Docker networking mode
  name: networkMode
  type: string
- description: Number of cpu units
  name: cpu
  type: string
- description: Amount of memory in MiB
  name: memory
  type: string
- description: ARN of task execution role
  name: executionRoleArn
  type: string
- description: ARN of task IAM role
  name: taskRoleArn
  type: string
- description: Container definitions
  name: containerDefinitions
  type: array
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-task-definition-schema.json
slug: amazon-fargate-task-definition
source_filename: amazon-fargate-task-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-task-definition-schema.json\",\n  \"title\": \"TaskDefinition\",\n  \"description\": \"An Amazon ECS task definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskDefinitionArn\": {\n      \"type\": \"string\",\n      \"description\": \"Full ARN of the task definition\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:task-definition/my-fargate-task:1\"\n    },\n    \"family\": {\n      \"type\": \"string\",\n      \"description\": \"Family of the task definition\",\n      \"example\": \"my-fargate-task\"\n    },\n    \"revision\": {\n      \"type\": \"integer\",\n      \"description\": \"Revision number\",\n      \"example\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Task definition status\",\n      \"example\": \"ACTIVE\"\
  ,\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"DELETE_IN_PROGRESS\"\n      ]\n    },\n    \"requiresCompatibilities\": {\n      \"type\": \"array\",\n      \"description\": \"Launch types the task definition is compatible with\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"FARGATE\"\n      ]\n    },\n    \"networkMode\": {\n      \"type\": \"string\",\n      \"description\": \"Docker networking mode\",\n      \"example\": \"awsvpc\",\n      \"enum\": [\n        \"bridge\",\n        \"host\",\n        \"awsvpc\",\n        \"none\"\n      ]\n    },\n    \"cpu\": {\n      \"type\": \"string\",\n      \"description\": \"Number of cpu units\",\n      \"example\": \"256\"\n    },\n    \"memory\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of memory in MiB\",\n      \"example\": \"512\"\n    },\n    \"executionRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of task execution\
  \ role\",\n      \"example\": \"arn:aws:iam::123456789012:role/ecsTaskExecutionRole\"\n    },\n    \"taskRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of task IAM role\",\n      \"example\": \"arn:aws:iam::123456789012:role/ecsTaskRole\"\n    },\n    \"containerDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"Container definitions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ContainerDefinition\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-task-definition-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: TaskDefinition
---
