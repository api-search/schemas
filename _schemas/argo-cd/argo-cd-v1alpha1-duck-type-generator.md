---
description: DuckType defines a generator to match against clusters registered with ArgoCD.
layout: schema
name: v1alpha1DuckTypeGenerator
properties_list:
- description: ''
  name: configMapRef
  type: string
- description: ''
  name: labelSelector
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-duck-type-generator-schema.json
slug: argo-cd-v1alpha1-duck-type-generator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1DuckTypeGenerator
---
