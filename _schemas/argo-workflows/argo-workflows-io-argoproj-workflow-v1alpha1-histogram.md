---
description: Histogram is a Histogram prometheus metric
layout: schema
name: io.argoproj.workflow.v1alpha1.Histogram
properties_list:
- description: Buckets is a list of bucket divisors for the histogram
  name: buckets
  type: array
- description: Value is the value of the metric
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-histogram-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-histogram
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-histogram-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Histogram\",\n  \"description\": \"Histogram is a Histogram prometheus metric\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buckets\": {\n      \"description\": \"Buckets is a list of bucket divisors for the histogram\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Amount\"\n      }\n    },\n    \"value\": {\n      \"description\": \"Value is the value of the metric\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"value\",\n    \"buckets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-histogram-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Histogram
---
