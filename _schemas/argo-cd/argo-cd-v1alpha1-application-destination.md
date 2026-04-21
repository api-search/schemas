---
description: v1alpha1ApplicationDestination schema from Argo CD API
layout: schema
name: v1alpha1ApplicationDestination
properties_list:
- description: Name is an alternate way of specifying the target cluster by its symbolic name. This must be set if Server is not set.
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: Server specifies the URL of the target cluster's Kubernetes control plane API. This must be set if Name is not set.
  name: server
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-destination-schema.json
slug: argo-cd-v1alpha1-application-destination
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationDestination
---
