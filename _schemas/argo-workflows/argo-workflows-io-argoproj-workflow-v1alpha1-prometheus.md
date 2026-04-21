---
description: Prometheus is a prometheus metric to be emitted
layout: schema
name: io.argoproj.workflow.v1alpha1.Prometheus
properties_list:
- description: Counter is a counter metric
  name: counter
  type: object
- description: Gauge is a gauge metric
  name: gauge
  type: object
- description: Help is a string that describes the metric
  name: help
  type: string
- description: Histogram is a histogram metric
  name: histogram
  type: object
- description: Labels is a list of metric labels
  name: labels
  type: array
- description: Name is the name of the metric
  name: name
  type: string
- description: When is a conditional statement that decides when to emit the metric
  name: when
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-prometheus-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-prometheus
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Prometheus
---
