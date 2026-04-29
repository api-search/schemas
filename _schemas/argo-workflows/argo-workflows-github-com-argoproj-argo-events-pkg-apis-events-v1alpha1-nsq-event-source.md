---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource
properties_list:
- description: ''
  name: channel
  type: string
- description: ''
  name: connectionBackoff
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: hostAddress
  type: string
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: tls
  type: object
- description: Topic to subscribe to.
  name: topic
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nsq-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nsq-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nsq-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nsq-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"string\",\n      \"title\": \"Channel used for subscription\"\n    },\n    \"connectionBackoff\": {\n      \"title\": \"Backoff holds parameters applied to connection.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"hostAddress\": {\n      \"type\": \"string\",\n      \"title\": \"HostAddress is the address of the host for NSQ lookup\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the nsq client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topic\": {\n      \"description\": \"Topic to subscribe to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nsq-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NSQEventSource
---
