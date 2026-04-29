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
source_filename: argo-cd-v1-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-schema.json\",\n  \"title\": \"v1Event\",\n  \"description\": \"Event is a report of an event somewhere in the cluster.  Events\\nhave a limited retention time and triggers and messages may evolve\\nwith time.  Event consumers should not rely on the timing of an event\\nwith a given Reason reflecting a consistent underlying trigger, or the\\ncontinued existence of events with that Reason.  Events should be\\ntreated as informative, best-effort, supplemental data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"title\": \"What action was taken/failed regarding to the Regarding object.\\n+optional\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"title\": \"The number of times this event has\
  \ occurred.\\n+optional\"\n    },\n    \"eventTime\": {\n      \"$ref\": \"#/definitions/v1MicroTime\"\n    },\n    \"firstTimestamp\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"involvedObject\": {\n      \"$ref\": \"#/definitions/v1ObjectReference\"\n    },\n    \"lastTimestamp\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"A human-readable description of the status of this operation.\\nTODO: decide on maximum length.\\n+optional\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/v1ObjectMeta\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"title\": \"This should be a short, machine understandable string that gives the reason\\nfor the transition into the object's current status.\\nTODO: provide exact specification for format.\\n+optional\"\n    },\n    \"related\": {\n      \"$ref\": \"#/definitions/v1ObjectReference\"\n    },\n    \"reportingComponent\": {\n \
  \     \"type\": \"string\",\n      \"title\": \"Name of the controller that emitted this Event, e.g. `kubernetes.io/kubelet`.\\n+optional\"\n    },\n    \"reportingInstance\": {\n      \"type\": \"string\",\n      \"title\": \"ID of the controller instance, e.g. `kubelet-xyzf`.\\n+optional\"\n    },\n    \"series\": {\n      \"$ref\": \"#/definitions/v1EventSeries\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1EventSource\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Type of this event (Normal, Warning), new types could be added in the future\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-event-schema.json
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
