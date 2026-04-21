---
description: Gauge is a Gauge prometheus metric
layout: schema
name: io.argoproj.workflow.v1alpha1.Gauge
properties_list:
- description: Operation defines the operation to apply with value and the metrics' current value
  name: operation
  type: string
- description: Realtime emits this metric in real time if applicable
  name: realtime
  type: boolean
- description: 'Value is the value to be used in the operation with the metric''s current value. If no operation is set, value is the value of the metric MaxLength is an artificial limit to limit CEL validation costs '
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gauge-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-gauge
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Gauge
---
