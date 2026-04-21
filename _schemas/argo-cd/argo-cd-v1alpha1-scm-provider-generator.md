---
description: SCMProviderGenerator defines a generator that scrapes a SCMaaS API to find candidate repos.
layout: schema
name: v1alpha1SCMProviderGenerator
properties_list:
- description: ''
  name: awsCodeCommit
  type: object
- description: ''
  name: azureDevOps
  type: object
- description: ''
  name: bitbucket
  type: object
- description: ''
  name: bitbucketServer
  type: object
- description: Which protocol to use for the SCM URL. Default is provider-specific but ssh if possible. Not all providers necessarily support all protocols.
  name: cloneProtocol
  type: string
- description: Filters for which repos should be considered.
  name: filters
  type: array
- description: ''
  name: gitea
  type: object
- description: ''
  name: github
  type: object
- description: ''
  name: gitlab
  type: object
- description: Standard parameters.
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGenerator
---
