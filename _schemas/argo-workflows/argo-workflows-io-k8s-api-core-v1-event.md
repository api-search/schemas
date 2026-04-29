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
source_filename: argo-workflows-io-k8s-api-core-v1-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Event\",\n  \"description\": \"Event is a report of an event somewhere in the cluster.  Events have a limited retention time and triggers and messages may evolve with time.  Event consumers should not rely on the timing of an event with a given Reason reflecting a consistent underlying trigger, or the continued existence of events with that Reason.  Events should be treated as informative, best-effort, supplemental data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"What action was taken/failed regarding to the Regarding object.\",\n      \"type\": \"string\"\n    },\n    \"apiVersion\": {\n      \"description\": \"APIVersion defines the versioned schema of this representation\
  \ of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources\",\n      \"type\": \"string\"\n    },\n    \"count\": {\n      \"description\": \"The number of times this event has occurred.\",\n      \"type\": \"integer\"\n    },\n    \"eventTime\": {\n      \"description\": \"Time when this Event was first observed.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.MicroTime\"\n    },\n    \"firstTimestamp\": {\n      \"description\": \"The time at which the event was first recorded. (Time of server receipt is in TypeMeta.)\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"involvedObject\": {\n      \"description\": \"The object that this event is about.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ObjectReference\"\n    },\n    \"kind\": {\n \
  \     \"description\": \"Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\",\n      \"type\": \"string\"\n    },\n    \"lastTimestamp\": {\n      \"description\": \"The time at which the most recent occurrence of this event was recorded.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"message\": {\n      \"description\": \"A human-readable description of the status of this operation.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"description\": \"Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta\"\n    },\n    \"reason\"\
  : {\n      \"description\": \"This should be a short, machine understandable string that gives the reason for the transition into the object's current status.\",\n      \"type\": \"string\"\n    },\n    \"related\": {\n      \"description\": \"Optional secondary object for more complex actions.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ObjectReference\"\n    },\n    \"reportingComponent\": {\n      \"description\": \"Name of the controller that emitted this Event, e.g. `kubernetes.io/kubelet`.\",\n      \"type\": \"string\"\n    },\n    \"reportingInstance\": {\n      \"description\": \"ID of the controller instance, e.g. `kubelet-xyzf`.\",\n      \"type\": \"string\"\n    },\n    \"series\": {\n      \"description\": \"Data about the Event series this event represents or nil if it's a singleton Event.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.EventSeries\"\n    },\n    \"source\": {\n      \"description\": \"The component reporting this event. Should be a short\
  \ machine understandable string.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.EventSource\"\n    },\n    \"type\": {\n      \"description\": \"Type of this event (Normal, Warning), new types could be added in the future\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"metadata\",\n    \"involvedObject\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-event-schema.json
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
