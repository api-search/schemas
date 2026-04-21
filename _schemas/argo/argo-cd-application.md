---
description: An Argo CD Application represents a deployed set of Kubernetes resources managed through GitOps.
layout: schema
name: Application
properties_list:
- description: API version, always argoproj.io/v1alpha1.
  name: apiVersion
  type: string
- description: Resource kind, always Application.
  name: kind
  type: string
- description: Kubernetes object metadata.
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
schema_file: json-schema/argo-cd-application-schema.json
slug: argo-cd-application
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Application
---
