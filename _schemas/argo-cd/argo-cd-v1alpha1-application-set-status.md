---
description: v1alpha1ApplicationSetStatus schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetStatus
properties_list:
- description: ''
  name: applicationStatus
  type: array
- description: ''
  name: conditions
  type: array
- description: ''
  name: health
  type: object
- description: Resources is a list of Applications resources managed by this application set.
  name: resources
  type: array
- description: ResourcesCount is the total number of resources managed by this application set. The count may be higher than actual number of items in the Resources field when the number of managed resources exceeds
  name: resourcesCount
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-status-schema.json
slug: argo-cd-v1alpha1-application-set-status
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetStatus
---
