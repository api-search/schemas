---
description: HostResourceInfo represents resource usage details for a specific resource type on a host.
layout: schema
name: v1alpha1HostResourceInfo
properties_list:
- description: Capacity represents the total available capacity of this resource on the host.
  name: capacity
  type: integer
- description: RequestedByApp indicates the total amount of this resource requested by the application running on the host.
  name: requestedByApp
  type: integer
- description: RequestedByNeighbors indicates the total amount of this resource requested by other workloads on the same host.
  name: requestedByNeighbors
  type: integer
- description: ResourceName specifies the type of resource (e.g., CPU, memory, storage).
  name: resourceName
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-host-resource-info-schema.json
slug: argo-cd-v1alpha1-host-resource-info
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HostResourceInfo
---
