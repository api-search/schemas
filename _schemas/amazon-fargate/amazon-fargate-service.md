---
description: An Amazon ECS service
layout: schema
name: Service
properties_list:
- description: ARN of the service
  name: serviceArn
  type: string
- description: Name of the service
  name: serviceName
  type: string
- description: ARN of the cluster
  name: clusterArn
  type: string
- description: Task definition ARN or family:revision
  name: taskDefinition
  type: string
- description: Desired number of tasks
  name: desiredCount
  type: integer
- description: Number of running tasks
  name: runningCount
  type: integer
- description: Number of pending tasks
  name: pendingCount
  type: integer
- description: Service status
  name: status
  type: string
- description: Launch type
  name: launchType
  type: string
- description: ''
  name: networkConfiguration
  type: object
- description: Load balancer configurations
  name: loadBalancers
  type: array
- description: Service creation time
  name: createdAt
  type: string
- description: Tags
  name: tags
  type: array
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-service-schema.json
slug: amazon-fargate-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"An Amazon ECS service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the service\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:service/my-fargate-cluster/my-fargate-service\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service\",\n      \"example\": \"my-fargate-service\"\n    },\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the cluster\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:cluster/my-fargate-cluster\"\n    },\n    \"taskDefinition\": {\n      \"type\": \"string\",\n      \"description\": \"Task definition\
  \ ARN or family:revision\",\n      \"example\": \"my-fargate-task:1\"\n    },\n    \"desiredCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Desired number of tasks\",\n      \"example\": 2\n    },\n    \"runningCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of running tasks\",\n      \"example\": 2\n    },\n    \"pendingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pending tasks\",\n      \"example\": 0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Service status\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DRAINING\",\n        \"INACTIVE\"\n      ]\n    },\n    \"launchType\": {\n      \"type\": \"string\",\n      \"description\": \"Launch type\",\n      \"example\": \"FARGATE\"\n    },\n    \"networkConfiguration\": {\n      \"$ref\": \"#/components/schemas/NetworkConfiguration\"\n    },\n    \"loadBalancers\": {\n      \"type\": \"\
  array\",\n      \"description\": \"Load balancer configurations\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoadBalancer\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Service creation time\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-service-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: Service
---
