---
description: ApplicationTree represents the hierarchical structure of resources associated with an Argo CD application.
layout: schema
name: v1alpha1ApplicationTree
properties_list:
- description: Hosts provides a list of Kubernetes nodes that are running pods related to the application.
  name: hosts
  type: array
- description: Nodes contains a list of resources that are either directly managed by the application or are children of directly managed resources.
  name: nodes
  type: array
- description: OrphanedNodes contains resources that exist in the same namespace as the application but are not managed by it. This list is populated only if orphaned resource tracking is enabled in the application'
  name: orphanedNodes
  type: array
- description: ShardsCount represents the total number of shards the application tree is split into. This is used to distribute resource processing across multiple shards.
  name: shardsCount
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-tree-schema.json
slug: argo-cd-v1alpha1-application-tree
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationTree
---
