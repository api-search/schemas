---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource
properties_list:
- description: 'Yaml format Sarama config for Kafka connection. It follows the struct of sarama.Config. See https://github.com/IBM/sarama/blob/main/config.go e.g. consumer: fetch: min: 1 net: MaxOpenRequests: 5 +opti'
  name: config
  type: string
- description: Backoff holds parameters applied to connection.
  name: connectionBackoff
  type: object
- description: ''
  name: consumerGroup
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: limitEventsPerSecond
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: partition
  type: string
- description: ''
  name: sasl
  type: object
- description: ''
  name: schemaRegistry
  type: object
- description: ''
  name: tls
  type: object
- description: ''
  name: topic
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-event-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaEventSource
---
