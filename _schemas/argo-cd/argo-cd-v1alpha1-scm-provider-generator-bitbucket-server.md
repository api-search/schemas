---
description: SCMProviderGeneratorBitbucketServer defines connection info specific to Bitbucket Server.
layout: schema
name: v1alpha1SCMProviderGeneratorBitbucketServer
properties_list:
- description: Scan all branches instead of just the default branch.
  name: allBranches
  type: boolean
- description: The Bitbucket Server REST API URL to talk to. Required.
  name: api
  type: string
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: bearerToken
  type: object
- description: ''
  name: caRef
  type: object
- description: ''
  name: insecure
  type: boolean
- description: Project to scan. Required.
  name: project
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-bitbucket-server-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator-bitbucket-server
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGeneratorBitbucketServer
---
