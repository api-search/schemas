---
description: PullRequestGeneratorBitbucket defines connection info specific to Bitbucket.
layout: schema
name: v1alpha1PullRequestGeneratorBitbucket
properties_list:
- description: The Bitbucket REST API URL to talk to. If blank, uses https://api.bitbucket.org/2.0.
  name: api
  type: string
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: bearerToken
  type: object
- description: Workspace to scan. Required.
  name: owner
  type: string
- description: Repo name to scan. Required.
  name: repo
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-bitbucket
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorBitbucket
---
