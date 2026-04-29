---
description: A Cluster represents a Kubernetes cluster connected to and managed by the CAST AI platform for cost optimization and autoscaling.
layout: schema
name: CAST AI Cluster
properties_list:
- description: Unique identifier for the cluster.
  name: id
  type: string
- description: Human-readable name of the cluster.
  name: name
  type: string
- description: Current status of the cluster.
  name: status
  type: string
- description: Cloud provider hosting the cluster.
  name: provider
  type: string
- description: Cloud provider region where the cluster is deployed.
  name: region
  type: string
- description: Token used by the CAST AI agent to authenticate with the platform.
  name: clusterToken
  type: string
- description: Status of the CAST AI agent running in the cluster.
  name: agentStatus
  type: string
- description: Version of Kubernetes running on the cluster.
  name: kubernetesVersion
  type: string
- description: Total number of nodes in the cluster.
  name: nodeCount
  type: integer
- description: Timestamp when the cluster was registered with CAST AI.
  name: createdAt
  type: string
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/cluster.json
slug: cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/cluster.json\",\n  \"title\": \"CAST AI Cluster\",\n  \"description\": \"A Cluster represents a Kubernetes cluster connected to and managed by the CAST AI platform for cost optimization and autoscaling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the cluster.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the cluster.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ready\",\n        \"connecting\",\n        \"disconnected\",\n        \"warning\",\n        \"deleting\"\n      ],\n      \"description\": \"Current status of the cluster.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"aws\",\n        \"gcp\",\n        \"azure\"\n      ],\n      \"description\": \"Cloud provider hosting the cluster.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider region where the cluster is deployed.\"\n    },\n    \"clusterToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token used by the CAST AI agent to authenticate with the platform.\"\n    },\n    \"agentStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"online\",\n        \"offline\"\n      ],\n      \"description\": \"Status of the CAST AI agent running in the cluster.\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of Kubernetes running on the cluster.\"\n    },\n    \"nodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of nodes in the cluster.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n   \
  \   \"description\": \"Timestamp when the cluster was registered with CAST AI.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/cluster.json
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Cluster
---
