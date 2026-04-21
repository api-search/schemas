---
description: v1alpha1ClusterResourceRestrictionItem schema from Argo CD API
layout: schema
name: v1alpha1ClusterResourceRestrictionItem
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: kind
  type: string
- description: Name is the name of the restricted resource. Glob patterns using Go's filepath.Match syntax are supported. Unlike the group and kind fields, if no name is specified, all resources of the specified gro
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-resource-restriction-item-schema.json
slug: argo-cd-v1alpha1-cluster-resource-restriction-item
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterResourceRestrictionItem
---
