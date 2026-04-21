---
description: TriggerTemplate is the template that describes trigger specification.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate
properties_list:
- description: ''
  name: argoWorkflow
  type: object
- description: ''
  name: awsLambda
  type: object
- description: ''
  name: azureEventHubs
  type: object
- description: ''
  name: azureServiceBus
  type: object
- description: ''
  name: conditions
  type: string
- description: ''
  name: conditionsReset
  type: array
- description: ''
  name: custom
  type: object
- description: ''
  name: email
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: k8s
  type: object
- description: Kafka refers to the trigger designed to place messages on Kafka topic. +optional.
  name: kafka
  type: object
- description: ''
  name: log
  type: object
- description: Name is a unique name of the action to take.
  name: name
  type: string
- description: NATS refers to the trigger designed to place message on NATS subject. +optional.
  name: nats
  type: object
- description: ''
  name: openWhisk
  type: object
- description: ''
  name: pulsar
  type: object
- description: ''
  name: slack
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate
---
