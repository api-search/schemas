---
description: A Node represents a Kubernetes node within a cluster managed by CAST AI, including its instance type, state, and labels.
layout: schema
name: CAST AI Node
properties_list:
- description: Unique identifier for the node.
  name: id
  type: string
- description: Name of the node.
  name: name
  type: string
- description: Cloud provider instance type of the node.
  name: instanceType
  type: string
- description: Current state of the node.
  name: state
  type: string
- description: Timestamp when the node was created.
  name: createdAt
  type: string
- description: Key-value labels assigned to the node.
  name: labels
  type: object
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/node.json
slug: node
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Node
---
