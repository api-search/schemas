---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource
properties_list:
- description: ''
  name: apiKey
  type: object
- description: ''
  name: createWebhook
  type: boolean
- description: ''
  name: eventFilter
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: webhook
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-stripe-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-stripe-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-stripe-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiKey\": {\n      \"title\": \"APIKey refers to K8s secret that holds Stripe API key. Used only if CreateWebhook is enabled.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"createWebhook\": {\n      \"type\": \"boolean\",\n      \"title\": \"CreateWebhook if specified creates a new webhook programmatically.\\n+optional\"\n    },\n    \"eventFilter\": {\n      \"type\": \"\
  array\",\n      \"title\": \"EventFilter describes the type of events to listen to. If not specified, all types of events will be processed.\\nMore info at https://stripe.com/docs/api/events/list\\n+optional\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"webhook\": {\n      \"title\": \"Webhook holds configuration for a REST endpoint\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WebhookContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-stripe-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StripeEventSource
---
