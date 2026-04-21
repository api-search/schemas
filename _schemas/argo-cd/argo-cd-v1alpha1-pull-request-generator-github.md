---
description: PullRequestGeneratorGithub defines connection info specific to GitHub.
layout: schema
name: v1alpha1PullRequestGeneratorGithub
properties_list:
- description: The GitHub API URL to talk to. If blank, use https://api.github.com/.
  name: api
  type: string
- description: AppSecretName is a reference to a GitHub App repo-creds secret with permission to access pull requests.
  name: appSecretName
  type: string
- description: ''
  name: labels
  type: array
- description: GitHub org or user to scan. Required.
  name: owner
  type: string
- description: GitHub repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-github-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-github
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGithub
---
