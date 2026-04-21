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
