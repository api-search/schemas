---
description: SCMProviderGeneratorGitea defines a connection info specific to Gitea.
layout: schema
name: v1alpha1SCMProviderGeneratorGitea
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Gitea URL to talk to. For example https://gitea.mydomain.com/.
  name: api
  type: string
- description: Exclude repositories that are archived.
  name: excludeArchivedRepos
  type: boolean
- description: ''
  name: insecure
  type: boolean
- description: Gitea organization or user to scan. Required.
  name: owner
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-gitea-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-gitea
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGitea
---
