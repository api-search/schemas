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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-prometheus-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Prometheus\",\n  \"description\": \"Prometheus is a prometheus metric to be emitted\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"counter\": {\n      \"description\": \"Counter is a counter metric\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Counter\"\n    },\n    \"gauge\": {\n      \"description\": \"Gauge is a gauge metric\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Gauge\"\n    },\n    \"help\": {\n      \"description\": \"Help is a string that describes the metric\",\n      \"type\": \"string\"\n    },\n    \"histogram\": {\n      \"description\": \"Histogram is a histogram metric\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Histogram\"\
  \n    },\n    \"labels\": {\n      \"description\": \"Labels is a list of metric labels\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.MetricLabel\"\n      }\n    },\n    \"name\": {\n      \"description\": \"Name is the name of the metric\",\n      \"type\": \"string\"\n    },\n    \"when\": {\n      \"description\": \"When is a conditional statement that decides when to emit the metric\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"help\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-prometheus-schema.json
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
