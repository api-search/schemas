---
description: Event is a report of an event somewhere in the cluster. Events have a limited retention time and triggers and messages may evolve with time. Event consumers should not rely on the timing of an event with a given Reason reflecting a consistent underlying trigger, or the continued existence of events with that Reason. Events should be treated as informative, best-effort, supplemental data.
layout: schema
name: v1Event
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: count
  type: integer
- description: ''
  name: eventTime
  type: object
- description: ''
  name: firstTimestamp
  type: object
- description: ''
  name: involvedObject
  type: object
- description: ''
  name: lastTimestamp
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: reason
  type: string
- description: ''
  name: related
  type: object
- description: ''
  name: reportingComponent
  type: string
- description: ''
  name: reportingInstance
  type: string
- description: ''
  name: series
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-event-schema.json
slug: argo-cd-v1-event
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1Event
---
