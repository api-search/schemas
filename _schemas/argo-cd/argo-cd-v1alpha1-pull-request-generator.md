---
description: PullRequestGenerator defines a generator that scrapes a PullRequest API to find candidate pull requests.
layout: schema
name: v1alpha1PullRequestGenerator
properties_list:
- description: ''
  name: azuredevops
  type: object
- description: ''
  name: bitbucket
  type: object
- description: ''
  name: bitbucketServer
  type: object
- description: ContinueOnRepoNotFoundError is a flag to continue the ApplicationSet Pull Request generator parameters generation even if the repository is not found.
  name: continueOnRepoNotFoundError
  type: boolean
- description: Filters for which pull requests should be considered.
  name: filters
  type: array
- description: ''
  name: gitea
  type: object
- description: ''
  name: github
  type: object
- description: ''
  name: gitlab
  type: object
- description: Standard parameters.
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
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-schema.json
slug: argo-cd-v1alpha1-pull-request-generator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGenerator
---
