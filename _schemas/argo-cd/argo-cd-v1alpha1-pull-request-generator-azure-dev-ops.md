---
description: PullRequestGeneratorAzureDevOps defines connection info specific to AzureDevOps.
layout: schema
name: v1alpha1PullRequestGeneratorAzureDevOps
properties_list:
- description: The Azure DevOps API URL to talk to. If blank, use https://dev.azure.com/.
  name: api
  type: string
- description: ''
  name: labels
  type: array
- description: Azure DevOps org to scan. Required.
  name: organization
  type: string
- description: Azure DevOps project name to scan. Required.
  name: project
  type: string
- description: Azure DevOps repo name to scan. Required.
  name: repo
  type: string
- description: ''
  name: tokenRef
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-azure-dev-ops-schema.json
slug: argo-cd-v1alpha1-pull-request-generator-azure-dev-ops
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGeneratorAzureDevOps
---
