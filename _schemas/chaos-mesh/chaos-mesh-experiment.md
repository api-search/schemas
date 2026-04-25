---
description: Schema for Chaos Mesh chaos experiment custom resources on Kubernetes. Covers all supported fault injection types including PodChaos, NetworkChaos, IOChaos, StressChaos, HTTPChaos, TimeChaos, DNSChaos, and KernelChaos. Each chaos type specifies a selector for targeting pods and a type-specific spec for the fault to inject.
layout: schema
name: Chaos Mesh Experiment
properties_list:
- description: Chaos Mesh API group and version for all chaos custom resources.
  name: apiVersion
  type: string
- description: Chaos type kind identifying which fault injector to use.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: Chaos experiment specification. The required fields and their meanings vary by kind. All chaos types share selector, mode, and duration fields.
  name: spec
  type: object
provider_name: Chaos Mesh
provider_slug: chaos-mesh
schema_file: json-schema/chaos-mesh-experiment-schema.json
slug: chaos-mesh-experiment
tags:
- Chaos Engineering
- Cloud Native
- CNCF
- Fault Injection
- Kubernetes
- Observability
- Open Source
- Reliability
- Resilience
- Testing
title: Chaos Mesh Experiment
---
