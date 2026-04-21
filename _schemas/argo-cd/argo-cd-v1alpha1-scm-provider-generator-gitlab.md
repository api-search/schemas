---
description: SCMProviderGeneratorGitlab defines connection info specific to Gitlab.
layout: schema
name: v1alpha1SCMProviderGeneratorGitlab
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Gitlab API URL to talk to.
  name: api
  type: string
- description: ''
  name: caRef
  type: object
- description: Gitlab group to scan. Required. You can use either the project id (recommended) or the full namespaced path.
  name: group
  type: string
- description: Include repositories that are archived.
  name: includeArchivedRepos
  type: boolean
- description: ''
  name: includeSharedProjects
  type: boolean
- description: ''
  name: includeSubgroups
  type: boolean
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: tokenRef
  type: object
- description: Filter repos list based on Gitlab Topic.
  name: topic
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-gitlab-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-gitlab
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGitlab
---
