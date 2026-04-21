---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource
properties_list:
- description: ''
  name: consumerGroup
  type: string
- description: ''
  name: db
  type: integer
- description: ''
  name: filter
  type: object
- description: ''
  name: hostAddress
  type: string
- description: ''
  name: maxMsgCountPerRead
  type: integer
- description: ''
  name: metadata
  type: object
- description: ''
  name: password
  type: object
- description: Streams to look for entries. XREADGROUP is used on all streams using a single consumer group.
  name: streams
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: username
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-redis-stream-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.RedisStreamEventSource
---
