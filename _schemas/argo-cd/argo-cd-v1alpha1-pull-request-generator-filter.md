---
description: PullRequestGeneratorFilter is a single pull request filter. If multiple filter types are set on a single struct, they will be AND'd together. All filters must pass for a pull request to be included.
layout: schema
name: v1alpha1PullRequestGeneratorFilter
properties_list:
- description: ''
  name: branchMatch
  type: string
- description: ''
  name: targetBranchMatch
  type: string
- description: ''
  name: titleMatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-filter-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-filter
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorFilter
---
