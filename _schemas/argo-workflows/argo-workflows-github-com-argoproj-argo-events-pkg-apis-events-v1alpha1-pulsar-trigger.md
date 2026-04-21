---
description: PulsarTrigger refers to the specification of the Pulsar trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger
properties_list:
- description: ''
  name: authAthenzParams
  type: object
- description: ''
  name: authAthenzSecret
  type: object
- description: ''
  name: authTokenSecret
  type: object
- description: ''
  name: connectionBackoff
  type: object
- description: Parameters is the list of parameters that is applied to resolved Kafka trigger object.
  name: parameters
  type: array
- description: Payload is the list of key-value extracted from an event payload to construct the request payload.
  name: payload
  type: array
- description: ''
  name: tls
  type: object
- description: ''
  name: tlsAllowInsecureConnection
  type: boolean
- description: ''
  name: tlsTrustCertsSecret
  type: object
- description: ''
  name: tlsValidateHostname
  type: boolean
- description: ''
  name: topic
  type: string
- description: ''
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pulsar-trigger
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger
---
