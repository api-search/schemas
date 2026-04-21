---
description: PullRequestGeneratorGitLab defines connection info specific to GitLab.
layout: schema
name: v1alpha1PullRequestGeneratorGitLab
properties_list:
- description: The GitLab API URL to talk to. If blank, uses https://gitlab.com/.
  name: api
  type: string
- description: ''
  name: caRef
  type: object
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: labels
  type: array
- description: GitLab project to scan. Required.
  name: project
  type: string
- description: 'PullRequestState is an additional MRs filter to get only those with a certain state. Default: "" (all states). Valid values: opened, closed, merged, locked".'
  name: pullRequestState
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-git-lab-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-git-lab
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorGitLab
---
