---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger
properties_list:
- description: ''
  name: fqdn
  type: string
- description: ''
  name: hubName
  type: string
- description: ''
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: sharedAccessKey
  type: object
- description: ''
  name: sharedAccessKeyName
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-event-hubs-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-event-hubs-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-event-hubs-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-event-hubs-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"title\": \"FQDN refers to the namespace dns of Azure Event Hubs to be used i.e. <namespace>.servicebus.windows.net\"\n    },\n    \"hubName\": {\n      \"type\": \"string\",\n      \"title\": \"HubName refers to the Azure Event Hub to send events to\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of key-value extracted\
  \ from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"sharedAccessKey\": {\n      \"title\": \"SharedAccessKey refers to a K8s secret containing the primary key for the\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"sharedAccessKeyName\": {\n      \"title\": \"SharedAccessKeyName refers to the name of the Shared Access Key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-event-hubs-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger
---
