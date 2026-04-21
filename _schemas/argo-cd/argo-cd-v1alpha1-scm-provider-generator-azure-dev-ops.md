---
description: SCMProviderGeneratorAzureDevOps defines connection info specific to Azure DevOps.
layout: schema
name: v1alpha1SCMProviderGeneratorAzureDevOps
properties_list:
- description: ''
  name: accessTokenRef
  type: object
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The URL to Azure DevOps. If blank, use https://dev.azure.com.
  name: api
  type: string
- description: Azure Devops organization. Required. E.g. "my-organization".
  name: organization
  type: string
- description: Azure Devops team project. Required. E.g. "my-team".
  name: teamProject
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-azure-dev-ops
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorAzureDevOps
---
