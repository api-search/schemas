---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource
properties_list:
- description: ''
  name: connectionString
  type: object
- description: DeferDelete controls when messages are removed from Azure Service Bus. If false (default), messages are received and deleted immediately before processing. If true, messages are locked and only delete
  name: deferDelete
  type: boolean
- description: ''
  name: filter
  type: object
- description: ''
  name: fullyQualifiedNamespace
  type: string
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
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
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionString\": {\n      \"title\": \"ConnectionString is the connection string for the Azure Service Bus. If this fields is not provided\\nit will try to access via Azure AD with DefaultAzureCredential and FullyQualifiedNamespace.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"deferDelete\": {\n      \"description\": \"DeferDelete controls\
  \ when messages are removed from Azure Service Bus.\\nIf false (default), messages are received and deleted immediately before processing.\\nIf true, messages are locked and only deleted after successful processing, ensuring they are not lost if processing fails.\",\n      \"type\": \"boolean\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"fullyQualifiedNamespace\": {\n      \"type\": \"string\",\n      \"title\": \"FullyQualifiedNamespace is the Service Bus namespace name (ex: myservicebus.servicebus.windows.net). This field is necessary to\\naccess via Azure AD (managed identity) and it is ignored if ConnectionString is set.\\n+optional\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\"\
  : {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queueName\": {\n      \"type\": \"string\",\n      \"title\": \"QueueName is the name of the Azure Service Bus Queue\"\n    },\n    \"subscriptionName\": {\n      \"type\": \"string\",\n      \"title\": \"SubscriptionName is the name of the Azure Service Bus Topic Subscription\"\n    },\n    \"tls\": {\n      \"title\": \"TLS configuration for the service bus client\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TLSConfig\"\n    },\n    \"topicName\": {\n      \"type\": \"string\",\n      \"title\": \"TopicName is the name of the Azure Service Bus Topic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-service-bus-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusEventSource
---
