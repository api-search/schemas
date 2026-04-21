---
description: A step in a steps template
layout: schema
name: WorkflowStep
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: template
  type: string
- description: ''
  name: arguments
  type: object
- description: ''
  name: when
  type: string
- description: ''
  name: withItems
  type: array
- description: ''
  name: withParam
  type: string
- description: ''
  name: continueOn
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-step-schema.json
slug: argo-workflows-workflow-step
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowStep
---
