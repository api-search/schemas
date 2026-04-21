---
description: A task in a DAG template
layout: schema
name: DAGTask
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
  name: dependencies
  type: array
- description: Conditional expression for task execution
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
schema_file: json-schema/argo-workflows-dag-task-schema.json
slug: argo-workflows-dag-task
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: DAGTask
---
