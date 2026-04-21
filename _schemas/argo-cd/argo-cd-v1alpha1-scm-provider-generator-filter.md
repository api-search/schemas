---
description: SCMProviderGeneratorFilter is a single repository filter. If multiple filter types are set on a single struct, they will be AND'd together. All filters must pass for a repo to be included.
layout: schema
name: v1alpha1SCMProviderGeneratorFilter
properties_list:
- description: A regex which must match the branch name.
  name: branchMatch
  type: string
- description: A regex which must match at least one label.
  name: labelMatch
  type: string
- description: An array of paths, all of which must not exist.
  name: pathsDoNotExist
  type: array
- description: An array of paths, all of which must exist.
  name: pathsExist
  type: array
- description: A regex for repo names.
  name: repositoryMatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-filter-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-filter
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorFilter
---
