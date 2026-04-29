---
description: An Amazon ECS task running on Fargate
layout: schema
name: Task
properties_list:
- description: ARN of the task
  name: taskArn
  type: string
- description: ARN of the cluster
  name: clusterArn
  type: string
- description: ARN of the task definition
  name: taskDefinitionArn
  type: string
- description: Last known status
  name: lastStatus
  type: string
- description: Desired status
  name: desiredStatus
  type: string
- description: Launch type
  name: launchType
  type: string
- description: CPU units
  name: cpu
  type: string
- description: Memory in MiB
  name: memory
  type: string
- description: Time task was created
  name: createdAt
  type: string
- description: Time task started running
  name: startedAt
  type: string
- description: Time task stopped
  name: stoppedAt
  type: string
- description: Reason task stopped
  name: stoppedReason
  type: string
- description: Network interfaces
  name: networkInterfaces
  type: array
- description: Tags
  name: tags
  type: array
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-task-schema.json
slug: amazon-fargate-task
source_filename: amazon-fargate-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"An Amazon ECS task running on Fargate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the task\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:task/my-fargate-cluster/abc123\"\n    },\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the cluster\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:cluster/my-fargate-cluster\"\n    },\n    \"taskDefinitionArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the task definition\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:task-definition/my-fargate-task:1\"\n    },\n    \"lastStatus\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Last known status\",\n      \"example\": \"RUNNING\",\n      \"enum\": [\n        \"PROVISIONING\",\n        \"PENDING\",\n        \"ACTIVATING\",\n        \"RUNNING\",\n        \"DEACTIVATING\",\n        \"STOPPING\",\n        \"DEPROVISIONING\",\n        \"STOPPED\",\n        \"DELETED\"\n      ]\n    },\n    \"desiredStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Desired status\",\n      \"example\": \"RUNNING\"\n    },\n    \"launchType\": {\n      \"type\": \"string\",\n      \"description\": \"Launch type\",\n      \"example\": \"FARGATE\",\n      \"enum\": [\n        \"EC2\",\n        \"FARGATE\",\n        \"EXTERNAL\"\n      ]\n    },\n    \"cpu\": {\n      \"type\": \"string\",\n      \"description\": \"CPU units\",\n      \"example\": \"256\"\n    },\n    \"memory\": {\n      \"type\": \"string\",\n      \"description\": \"Memory in MiB\",\n      \"example\": \"512\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"date-time\",\n      \"description\": \"Time task was created\",\n      \"example\": \"2026-04-19T12:00:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time task started running\",\n      \"example\": \"2026-04-19T12:00:30Z\"\n    },\n    \"stoppedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time task stopped\"\n    },\n    \"stoppedReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason task stopped\"\n    },\n    \"networkInterfaces\": {\n      \"type\": \"array\",\n      \"description\": \"Network interfaces\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-task-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: Task
---
