---
description: ResourceEventSource refers to a event-source for K8s resource related events.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceEventSource
properties_list:
- description: EventTypes is the list of event type to watch. Possible values are - ADD, UPDATE and DELETE.
  name: eventTypes
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: groupVersionResource
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceEventSource
---
