---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger
properties_list:
- description: ''
  name: connectionString
  type: object
- description: ''
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: queueName
  type: string
- description: ''
  name: subscriptionName
  type: string
- description: ''
  name: tls
  type: object
- description: ''
  name: topicName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionString\": {\n      \"title\": \"ConnectionString is the connection string for the Azure Service Bus\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n \
  \       \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"payload\": {\n      \"description\": \"Payload is the list of key-value extracted from an event payload to construct the request payload.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"queueName\": {\n      \"type\": \"string\",\n      \"title\": \"QueueName is the name of the Azure Service Bus Queue\"\n    },\n    \"subscriptionName\": {\n      \"type\": \"string\",\n      \"title\": \"SubscriptionName is the name of the Azure Service Bus Topic Subscription\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the service bus client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topicName\": {\n      \"type\": \"string\"\
  ,\n      \"title\": \"TopicName is the name of the Azure Service Bus Topic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger
---
