---
description: JSON Schema for the Argo Rollouts Rollout CRD, which enables progressive delivery strategies including canary and blue-green deployments with automated traffic management and analysis.
layout: schema
name: Argo Rollout Spec
properties_list:
- description: API version for Argo Rollouts resources.
  name: apiVersion
  type: string
- description: Resource kind for Argo Rollouts.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-rollout-schema.json
slug: argo-rollout
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Argo Rollout Spec
---
