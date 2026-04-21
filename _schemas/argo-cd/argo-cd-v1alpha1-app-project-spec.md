---
description: v1alpha1AppProjectSpec schema from Argo CD API
layout: schema
name: v1alpha1AppProjectSpec
properties_list:
- description: ''
  name: clusterResourceBlacklist
  type: array
- description: ''
  name: clusterResourceWhitelist
  type: array
- description: ''
  name: description
  type: string
- description: DestinationServiceAccounts holds information about the service accounts to be impersonated for the application sync operation for each destination.
  name: destinationServiceAccounts
  type: array
- description: ''
  name: destinations
  type: array
- description: ''
  name: namespaceResourceBlacklist
  type: array
- description: ''
  name: namespaceResourceWhitelist
  type: array
- description: ''
  name: orphanedResources
  type: object
- description: ''
  name: permitOnlyProjectScopedClusters
  type: boolean
- description: ''
  name: roles
  type: array
- description: ''
  name: signatureKeys
  type: array
- description: ''
  name: sourceNamespaces
  type: array
- description: ''
  name: sourceRepos
  type: array
- description: ''
  name: syncWindows
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-app-project-spec-schema.json
slug: argo-cd-v1alpha1-app-project-spec
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AppProjectSpec
---
