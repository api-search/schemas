---
description: HostInfo holds metadata and resource usage metrics for a specific host in the cluster.
layout: schema
name: v1alpha1HostInfo
properties_list:
- description: Labels holds the labels attached to the host.
  name: labels
  type: object
- description: Name is the hostname or node name in the Kubernetes cluster.
  name: name
  type: string
- description: ResourcesInfo provides a list of resource usage details for different resource types on this host.
  name: resourcesInfo
  type: array
- description: ''
  name: systemInfo
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-host-info-schema.json
slug: argo-cd-v1alpha1-host-info
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HostInfo
---
