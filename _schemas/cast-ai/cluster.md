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
