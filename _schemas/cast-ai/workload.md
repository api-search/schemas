---
description: A Workload represents a Kubernetes workload monitored by CAST AI for optimization, including resource requests and recommendations.
layout: schema
name: CAST AI Workload
properties_list:
- description: Unique identifier for the workload.
  name: id
  type: string
- description: ID of the cluster the workload belongs to.
  name: clusterId
  type: string
- description: Kubernetes namespace of the workload.
  name: namespace
  type: string
- description: Name of the workload.
  name: name
  type: string
- description: Kubernetes workload type.
  name: type
  type: string
- description: Containers within the workload.
  name: containers
  type: array
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/workload.json
slug: workload
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Workload
---
