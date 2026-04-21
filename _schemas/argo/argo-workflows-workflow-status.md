---
description: Status of a workflow execution
layout: schema
name: WorkflowStatus
properties_list:
- description: ''
  name: phase
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: Progress of the workflow (e.g. 2/4)
  name: progress
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: estimatedDuration
  type: integer
- description: ''
  name: nodes
  type: object
- description: ''
  name: conditions
  type: array
- description: ''
  name: outputs
  type: object
- description: ''
  name: storedTemplates
  type: object
- description: ''
  name: artifactRepositoryRef
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-status-schema.json
slug: argo-workflows-workflow-status
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowStatus
---
