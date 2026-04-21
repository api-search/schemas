---
description: PullRequestGeneratorGitea defines connection info specific to Gitea.
layout: schema
name: v1alpha1PullRequestGeneratorGitea
properties_list:
- description: ''
  name: api
  type: string
- description: 'Allow insecure tls, for self-signed certificates; default: false.'
  name: insecure
  type: boolean
- description: ''
  name: labels
  type: array
- description: Gitea org or user to scan. Required.
  name: owner
  type: string
- description: Gitea repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-gitea-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-gitea
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGitea
---
