---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext
properties_list:
- description: ''
  name: authSecret
  type: object
- description: ''
  name: endpoint
  type: string
- description: ''
  name: maxPayloadSize
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: method
  type: string
- description: Port on which HTTP server is listening for incoming events.
  name: port
  type: string
- description: ServerCertPath refers the file that contains the cert.
  name: serverCertSecret
  type: object
- description: ''
  name: serverKeySecret
  type: object
- description: URL is the url of the server.
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-webhook-context-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-webhook-context
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-webhook-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-webhook-context-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authSecret\": {\n      \"title\": \"AuthSecret holds a secret selector that contains a bearer token for authentication\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"title\": \"REST API endpoint\"\n    },\n    \"maxPayloadSize\": {\n      \"type\": \"string\",\n      \"title\": \"MaxPayloadSize is the maximum webhook payload size\
  \ that the server will accept.\\nRequests exceeding that limit will be rejected with \\\"request too large\\\" response.\\nDefault value: 1048576 (1MB).\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"title\": \"Method is HTTP request method that indicates the desired action to be performed for a given resource.\\nSee RFC7231 Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content\"\n    },\n    \"port\": {\n      \"description\": \"Port on which HTTP server is listening for incoming events.\",\n      \"type\": \"string\"\n    },\n    \"serverCertSecret\": {\n      \"description\": \"ServerCertPath refers the file that contains the cert.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    },\n    \"serverKeySecret\": {\n      \"title\": \"ServerKeyPath refers the file that contains private key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"url\": {\n      \"description\": \"URL is the url of the server.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-webhook-context-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext
---
