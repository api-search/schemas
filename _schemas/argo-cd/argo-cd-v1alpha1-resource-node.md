---
description: ResourceNode contains information about a live Kubernetes resource and its relationships with other resources.
layout: schema
name: v1alpha1ResourceNode
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: health
  type: object
- description: Images lists container images associated with the resource. This is primarily useful for pods and other workload resources.
  name: images
  type: array
- description: Info provides additional metadata or annotations about the resource.
  name: info
  type: array
- description: ''
  name: networkingInfo
  type: object
- description: ParentRefs lists the parent resources that reference this resource. This helps in understanding ownership and hierarchical relationships.
  name: parentRefs
  type: array
- description: ResourceVersion indicates the version of the resource, used to track changes.
  name: resourceVersion
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-node-schema.json
slug: argo-cd-v1alpha1-resource-node
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceNode
---
