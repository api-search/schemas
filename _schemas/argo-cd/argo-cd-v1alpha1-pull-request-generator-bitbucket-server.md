---
description: PullRequestGeneratorBitbucketServer defines connection info specific to BitbucketServer.
layout: schema
name: v1alpha1PullRequestGeneratorBitbucketServer
properties_list:
- description: The Bitbucket REST API URL to talk to e.g. https://bitbucket.org/rest Required.
  name: api
  type: string
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: bearerToken
  type: object
- description: ''
  name: caRef
  type: object
- description: ''
  name: insecure
  type: boolean
- description: Project to scan. Required.
  name: project
  type: string
- description: Repo name to scan. Required.
  name: repo
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-bitbucket-server-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-bitbucket-server
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorBitbucketServer
---
