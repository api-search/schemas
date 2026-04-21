---
description: ResourceNetworkingInfo holds networking-related information for a resource.
layout: schema
name: v1alpha1ResourceNetworkingInfo
properties_list:
- description: ExternalURLs holds a list of URLs that should be accessible externally. This field is typically populated for Ingress resources based on their hostname rules.
  name: externalURLs
  type: array
- description: Ingress provides information about external access points (e.g., load balancer ingress) for this resource.
  name: ingress
  type: array
- description: Labels holds the labels associated with this networking resource.
  name: labels
  type: object
- description: TargetLabels represents labels associated with the target resources that this resource communicates with.
  name: targetLabels
  type: object
- description: TargetRefs contains references to other resources that this resource interacts with, such as Services or Pods.
  name: targetRefs
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-networking-info-schema.json
slug: argo-cd-v1alpha1-resource-networking-info
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceNetworkingInfo
---
