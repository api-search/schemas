---
description: SCMProviderGeneratorGithub defines connection info specific to GitHub.
layout: schema
name: v1alpha1SCMProviderGeneratorGithub
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The GitHub API URL to talk to. If blank, use https://api.github.com/.
  name: api
  type: string
- description: AppSecretName is a reference to a GitHub App repo-creds secret.
  name: appSecretName
  type: string
- description: Exclude repositories that are archived.
  name: excludeArchivedRepos
  type: boolean
- description: GitHub org to scan. Required.
  name: organization
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-github-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-github
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorGithub
---
