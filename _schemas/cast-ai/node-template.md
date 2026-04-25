---
description: A Node Template defines instance type constraints and configuration for nodes provisioned by the CAST AI autoscaler.
layout: schema
name: CAST AI Node Template
properties_list:
- description: Unique identifier for the node template.
  name: id
  type: string
- description: Name of the node template.
  name: name
  type: string
- description: ID of the associated node configuration.
  name: configurationId
  type: string
- description: Resource constraints for node selection.
  name: constraints
  type: object
- description: Timestamp when the node template was created.
  name: createdAt
  type: string
- description: Timestamp when the node template was last updated.
  name: updatedAt
  type: string
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/node-template.json
slug: node-template
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Node Template
---
