---
description: SCMProviderGeneratorBitbucket defines connection info specific to Bitbucket Cloud (API version 2).
layout: schema
name: v1alpha1SCMProviderGeneratorBitbucket
properties_list:
- description: Scan all branches instead of just the main branch.
  name: allBranches
  type: boolean
- description: ''
  name: appPasswordRef
  type: object
- description: Bitbucket workspace to scan. Required.
  name: owner
  type: string
- description: ''
  name: user
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-bitbucket
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorBitbucket
---
