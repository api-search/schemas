---
description: v1alpha1Cluster schema from Argo CD API
layout: schema
name: v1alpha1Cluster
properties_list:
- description: ''
  name: annotations
  type: object
- description: Indicates if cluster level resources should be managed. This setting is used only if cluster is connected in a namespaced mode.
  name: clusterResources
  type: boolean
- description: ''
  name: config
  type: object
- description: ''
  name: connectionState
  type: object
- description: ''
  name: info
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: name
  type: string
- description: Holds list of namespaces which are accessible in that cluster. Cluster level resources will be ignored if namespace list is not empty.
  name: namespaces
  type: array
- description: ''
  name: project
  type: string
- description: ''
  name: refreshRequestedAt
  type: object
- description: ''
  name: server
  type: string
- description: ''
  name: serverVersion
  type: string
- description: Shard contains optional shard number. Calculated on the fly by the application controller if not specified.
  name: shard
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-schema.json
slug: argo-cd-v1alpha1-cluster
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Cluster
---
