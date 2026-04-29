---
description: ''
layout: schema
name: CreateClusterRequest
properties_list:
- description: The name of the cluster to create (up to 255 characters). If not specified, the default cluster is created.
  name: clusterName
  type: string
- description: The short names of capacity providers to associate with the cluster.
  name: capacityProviders
  type: array
- description: The default capacity provider strategy for the cluster.
  name: defaultCapacityProviderStrategy
  type: array
- description: The cluster settings (e.g., Container Insights).
  name: settings
  type: array
- description: Metadata tags to apply to the cluster (up to 50).
  name: tags
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-create-cluster-request-schema.json
slug: amazon-ecs-create-cluster-request
source_filename: amazon-ecs-create-cluster-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateClusterRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster to create (up to 255 characters). If not specified, the default cluster is created.\"\n    },\n    \"capacityProviders\": {\n      \"type\": \"array\",\n      \"description\": \"The short names of capacity providers to associate with the cluster.\"\n    },\n    \"defaultCapacityProviderStrategy\": {\n      \"type\": \"array\",\n      \"description\": \"The default capacity provider strategy for the cluster.\"\n    },\n    \"settings\": {\n      \"type\": \"array\",\n      \"description\": \"The cluster settings (e.g., Container Insights).\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Metadata tags to apply to the cluster (up to 50).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-create-cluster-request-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: CreateClusterRequest
---
