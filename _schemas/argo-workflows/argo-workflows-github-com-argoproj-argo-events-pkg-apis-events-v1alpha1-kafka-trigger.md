---
description: KafkaTrigger refers to the specification of the Kafka trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger
properties_list:
- description: ''
  name: compress
  type: boolean
- description: ''
  name: flushFrequency
  type: integer
- description: ''
  name: headers
  type: object
- description: Parameters is the list of parameters that is applied to resolved Kafka trigger object.
  name: parameters
  type: array
- description: ''
  name: partition
  type: integer
- description: The partitioning key for the messages put on the Kafka topic. +optional.
  name: partitioningKey
  type: string
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: RequiredAcks used in producer to tell the broker how many replica acknowledgements Defaults to 1 (Only wait for the leader to ack). +optional.
  name: requiredAcks
  type: integer
- description: ''
  name: sasl
  type: object
- description: ''
  name: schemaRegistry
  type: object
- description: ''
  name: secureHeaders
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: topic
  type: string
- description: URL of the Kafka broker, multiple URLs separated by comma.
  name: url
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-kafka-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger
---
