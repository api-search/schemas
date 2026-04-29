---
description: GenericEventSource refers to a generic event source. It can be used to implement a custom event source.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GenericEventSource
properties_list:
- description: ''
  name: authSecret
  type: object
- description: ''
  name: config
  type: string
- description: ''
  name: filter
  type: object
- description: Insecure determines the type of connection.
  name: insecure
  type: boolean
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: URL of the gRPC server that implements the event source.
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-generic-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-generic-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-generic-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GenericEventSource\",\n  \"description\": \"GenericEventSource refers to a generic event source. It can be used to implement a custom event source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authSecret\": {\n      \"title\": \"AuthSecret holds a secret selector that contains a bearer token for authentication\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"config\": {\n      \"type\": \"string\",\n      \"title\": \"Config is the event source configuration\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"insecure\": {\n      \"description\": \"Insecure determines the type of connection.\",\n      \"type\": \"boolean\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"url\": {\n      \"description\": \"URL of the gRPC server that implements the event source.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-generic-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GenericEventSource
---
