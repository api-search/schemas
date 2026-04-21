---
description: Event is a report of an event somewhere in the cluster. Events have a limited retention time and triggers and messages may evolve with time. Event consumers should not rely on the timing of an event with a given Reason reflecting a consistent underlying trigger, or the continued existence of events with that Reason. Events should be treated as informative, best-effort, supplemental data.
layout: schema
name: io.k8s.api.core.v1.Event
properties_list:
- description: What action was taken/failed regarding to the Regarding object.
  name: action
  type: string
- description: 'APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: http'
  name: apiVersion
  type: string
- description: The number of times this event has occurred.
  name: count
  type: integer
- description: Time when this Event was first observed.
  name: eventTime
  type: object
- description: The time at which the event was first recorded. (Time of server receipt is in TypeMeta.)
  name: firstTimestamp
  type: object
- description: The object that this event is about.
  name: involvedObject
  type: object
- description: 'Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https'
  name: kind
  type: string
- description: The time at which the most recent occurrence of this event was recorded.
  name: lastTimestamp
  type: object
- description: A human-readable description of the status of this operation.
  name: message
  type: string
- description: 'Standard object''s metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata'
  name: metadata
  type: object
- description: This should be a short, machine understandable string that gives the reason for the transition into the object's current status.
  name: reason
  type: string
- description: Optional secondary object for more complex actions.
  name: related
  type: object
- description: Name of the controller that emitted this Event, e.g. `kubernetes.io/kubelet`.
  name: reportingComponent
  type: string
- description: ID of the controller instance, e.g. `kubelet-xyzf`.
  name: reportingInstance
  type: string
- description: Data about the Event series this event represents or nil if it's a singleton Event.
  name: series
  type: object
- description: The component reporting this event. Should be a short machine understandable string.
  name: source
  type: object
- description: Type of this event (Normal, Warning), new types could be added in the future
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-event-schema.json
slug: argo-workflows-io-k8s-api-core-v1-event
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Event
---
