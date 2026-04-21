---
description: DrySource specifies a location for dry "don't repeat yourself" manifest source information.
layout: schema
name: v1alpha1DrySource
properties_list:
- description: ''
  name: directory
  type: object
- description: ''
  name: helm
  type: object
- description: ''
  name: kustomize
  type: object
- description: ''
  name: path
  type: string
- description: ''
  name: plugin
  type: object
- description: ''
  name: repoURL
  type: string
- description: ''
  name: targetRevision
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-dry-source-schema.json
slug: argo-cd-v1alpha1-dry-source
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1DrySource
---
