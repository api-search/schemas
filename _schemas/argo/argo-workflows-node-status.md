---
description: Status of a workflow node
layout: schema
name: NodeStatus
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: templateName
  type: string
- description: ''
  name: phase
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: children
  type: array
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-node-status-schema.json
slug: argo-workflows-node-status
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: NodeStatus
---
