---
description: v1alpha1ApplicationSetApplicationStatus schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetApplicationStatus
properties_list:
- description: ''
  name: application
  type: string
- description: ''
  name: lastTransitionTime
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: step
  type: string
- description: TargetRevision tracks the desired revisions the Application should be synced to.
  name: targetrevisions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-application-status-schema.json
slug: argo-cd-v1alpha1-application-set-application-status
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetApplicationStatus
---
