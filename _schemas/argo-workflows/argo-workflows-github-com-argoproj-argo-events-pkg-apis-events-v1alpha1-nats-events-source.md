---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource
properties_list:
- description: ''
  name: auth
  type: object
- description: ConnectionBackoff holds backoff applied to connection.
  name: connectionBackoff
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: queue
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: tls
  type: object
- description: ''
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-events-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-events-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-events-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-events-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth\": {\n      \"title\": \"Auth information\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSAuth\"\n    },\n    \"connectionBackoff\": {\n      \"description\": \"ConnectionBackoff holds backoff applied to connection.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Backoff\"\n    },\n    \"filter\": {\n      \"title\": \"\
  Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queue\": {\n      \"type\": \"string\",\n      \"title\": \"Queue is the name of the queue group to subscribe as if specified. Uses QueueSubscribe\\nlogic to subscribe as queue group. If the queue is empty, uses default Subscribe logic.\\n+optional\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"title\": \"Subject holds the name of the subject onto which messages are published\"\n    },\n    \"tls\"\
  : {\n      \"title\": \"TLS configuration for the nats client.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"title\": \"URL to connect to NATS cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-nats-events-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSEventsSource
---
