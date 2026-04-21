---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventContext schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventContext
properties_list:
- description: DataContentType - A MIME (RFC2046) string describing the media type of `data`.
  name: datacontenttype
  type: string
- description: ID of the event; must be non-empty and unique within the scope of the producer.
  name: id
  type: string
- description: Source - A URI describing the event producer.
  name: source
  type: string
- description: SpecVersion - The version of the CloudEvents specification used by the io.argoproj.workflow.v1alpha1.
  name: specversion
  type: string
- description: ''
  name: subject
  type: string
- description: Time - A Timestamp when the event happened.
  name: time
  type: object
- description: Type - The type of the occurrence which has happened.
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-context-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-context
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventContext
---
