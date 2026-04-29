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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceEventSource\",\n  \"description\": \"ResourceEventSource refers to a event-source for K8s resource related events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypes\": {\n      \"description\": \"EventTypes is the list of event type to watch.\\nPossible values are - ADD, UPDATE and DELETE.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"title\": \"Filter is applied on the metadata of the resource\\nIf you apply filter, then the internal event informer will only monitor objects that pass the filter.\\n+optional\",\n      \"\
  $ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter\"\n    },\n    \"groupVersionResource\": {\n      \"title\": \"Group of the resource\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.GroupVersionResource\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace where resource is deployed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-event-source-schema.json
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
