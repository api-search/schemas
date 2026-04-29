---
description: Metrics are a list of metrics emitted from a Workflow/Template
layout: schema
name: io.argoproj.workflow.v1alpha1.Metrics
properties_list:
- description: Prometheus is a list of prometheus metrics to be emitted MaxItems is an artificial limit to limit CEL validation costs - see note at top of file
  name: prometheus
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-metrics-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-metrics
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-metrics-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Metrics\",\n  \"description\": \"Metrics are a list of metrics emitted from a Workflow/Template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prometheus\": {\n      \"description\": \"Prometheus is a list of prometheus metrics to be emitted MaxItems is an artificial limit to limit CEL validation costs - see note at top of file\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Prometheus\"\n      }\n    }\n  },\n  \"required\": [\n    \"prometheus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-metrics-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Metrics
---
