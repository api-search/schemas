---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource
properties_list:
- description: APIURL is the url of the storagegrid api.
  name: apiURL
  type: string
- description: ''
  name: authToken
  type: object
- description: Name of the bucket to register notifications for.
  name: bucket
  type: string
- description: ''
  name: events
  type: array
- description: Filter on object key which caused the notification.
  name: filter
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: region
  type: string
- description: ''
  name: tls
  type: object
- description: ''
  name: topicArn
  type: string
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-storage-grid-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-storage-grid-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-storage-grid-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-storage-grid-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiURL\": {\n      \"description\": \"APIURL is the url of the storagegrid api.\",\n      \"type\": \"string\"\n    },\n    \"authToken\": {\n      \"title\": \"Auth token for storagegrid api\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"bucket\": {\n      \"description\": \"Name of the bucket to register notifications for.\",\n      \"type\": \"string\"\n    },\n  \
  \  \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"description\": \"Filter on object key which caused the notification.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridFilter\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"title\": \"S3 region.\\nDefaults to us-east-1\\n+optional\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the service bus client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topicArn\": {\n      \"type\": \"string\",\n      \"title\": \"TopicArn\"\n    },\n\
  \    \"webhook\": {\n      \"title\": \"Webhook holds configuration for a REST endpoint\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-storage-grid-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StorageGridEventSource
---
