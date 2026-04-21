---
description: ClusterGenerator defines a generator to match against clusters registered with ArgoCD.
layout: schema
name: v1alpha1ClusterGenerator
properties_list:
- description: ''
  name: flatList
  type: boolean
- description: ''
  name: selector
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-generator-schema.json
slug: argo-cd-v1alpha1-cluster-generator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterGenerator
---
