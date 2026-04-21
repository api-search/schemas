---
description: SCMProviderGeneratorAWSCodeCommit defines connection info specific to AWS CodeCommit.
layout: schema
name: v1alpha1SCMProviderGeneratorAWSCodeCommit
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: Region provides the AWS region to discover repos. if not provided, AppSet controller will infer the current region from environment.
  name: region
  type: string
- description: Role provides the AWS IAM role to assume, for cross-account repo discovery if not provided, AppSet controller will use its pod/node identity to discover.
  name: role
  type: string
- description: ''
  name: tagFilters
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-aws-code-commit-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-aws-code-commit
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorAWSCodeCommit
---
