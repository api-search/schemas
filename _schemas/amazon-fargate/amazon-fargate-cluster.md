---
description: An Amazon ECS cluster
layout: schema
name: Cluster
properties_list:
- description: The ARN of the cluster
  name: clusterArn
  type: string
- description: The name of the cluster
  name: clusterName
  type: string
- description: Cluster status
  name: status
  type: string
- description: Number of registered container instances
  name: registeredContainerInstancesCount
  type: integer
- description: Number of running tasks
  name: runningTasksCount
  type: integer
- description: Number of pending tasks
  name: pendingTasksCount
  type: integer
- description: Number of active services
  name: activeServicesCount
  type: integer
- description: Tags associated with the cluster
  name: tags
  type: array
- description: Cluster settings
  name: settings
  type: array
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-cluster-schema.json
slug: amazon-fargate-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"An Amazon ECS cluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the cluster\",\n      \"example\": \"arn:aws:ecs:us-east-1:123456789012:cluster/my-fargate-cluster\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster\",\n      \"example\": \"my-fargate-cluster\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster status\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PROVISIONING\",\n        \"DEPROVISIONING\",\n        \"FAILED\",\n        \"INACTIVE\"\n      ]\n    },\n    \"registeredContainerInstancesCount\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of registered container instances\",\n      \"example\": 0\n    },\n    \"runningTasksCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of running tasks\",\n      \"example\": 5\n    },\n    \"pendingTasksCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pending tasks\",\n      \"example\": 0\n    },\n    \"activeServicesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active services\",\n      \"example\": 2\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the cluster\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    },\n    \"settings\": {\n      \"type\": \"array\",\n      \"description\": \"Cluster settings\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClusterSetting\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-cluster-schema.json
tags:
- AWS
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: Cluster
---
