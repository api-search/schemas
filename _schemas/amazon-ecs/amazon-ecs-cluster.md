---
description: A regional grouping of one or more container instances on which you can run tasks and services.
layout: schema
name: Cluster
properties_list:
- description: The ARN that identifies the cluster.
  name: clusterArn
  type: string
- description: A user-generated string that you use to identify your cluster.
  name: clusterName
  type: string
- description: The status of the cluster.
  name: status
  type: string
- description: The number of container instances registered into the cluster.
  name: registeredContainerInstancesCount
  type: integer
- description: The number of tasks in the cluster that are in the RUNNING state.
  name: runningTasksCount
  type: integer
- description: The number of tasks in the cluster that are in the PENDING state.
  name: pendingTasksCount
  type: integer
- description: The number of services in the cluster that are in an ACTIVE state.
  name: activeServicesCount
  type: integer
- description: ''
  name: statistics
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: settings
  type: array
- description: ''
  name: capacityProviders
  type: array
- description: ''
  name: defaultCapacityProviderStrategy
  type: array
- description: ''
  name: attachments
  type: array
- description: ''
  name: attachmentsStatus
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-cluster-schema.json
slug: amazon-ecs-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cluster\",\n  \"type\": \"object\",\n  \"description\": \"A regional grouping of one or more container instances on which you can run tasks and services.\",\n  \"properties\": {\n    \"clusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN that identifies the cluster.\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-generated string that you use to identify your cluster.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the cluster.\"\n    },\n    \"registeredContainerInstancesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of container instances registered into the cluster.\"\n    },\n    \"runningTasksCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks in the cluster that are in the RUNNING state.\"\n    },\n\
  \    \"pendingTasksCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks in the cluster that are in the PENDING state.\"\n    },\n    \"activeServicesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of services in the cluster that are in an ACTIVE state.\"\n    },\n    \"statistics\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"settings\": {\n      \"type\": \"array\"\n    },\n    \"capacityProviders\": {\n      \"type\": \"array\"\n    },\n    \"defaultCapacityProviderStrategy\": {\n      \"type\": \"array\"\n    },\n    \"attachments\": {\n      \"type\": \"array\"\n    },\n    \"attachmentsStatus\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-cluster-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Cluster
---
