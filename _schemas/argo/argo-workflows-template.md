---
description: A workflow template definition
layout: schema
name: Template
properties_list:
- description: Name of the template
  name: name
  type: string
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: object
- description: Container to run
  name: container
  type: object
- description: Script to run in a container
  name: script
  type: object
- description: Kubernetes resource to create/patch/delete
  name: resource
  type: object
- description: DAG template definition
  name: dag
  type: object
- description: Steps template definition (list of parallel step groups)
  name: steps
  type: array
- description: Suspend template for manual approval
  name: suspend
  type: object
- description: ''
  name: activeDeadlineSeconds
  type: integer
- description: ''
  name: retryStrategy
  type: object
- description: ''
  name: nodeSelector
  type: object
- description: Metadata to set on step pods
  name: metadata
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-template-schema.json
slug: argo-workflows-template
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Template
---
