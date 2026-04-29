---
description: ContainerSetRetryStrategy provides controls on how to retry a container set
layout: schema
name: io.argoproj.workflow.v1alpha1.ContainerSetRetryStrategy
properties_list:
- description: Duration is the time between each retry, examples values are "300ms", "1s" or "5m". Valid time units are "ns", "us" (or "µs"), "ms", "s", "m", "h".
  name: duration
  type: string
- description: Retries is the maximum number of retry attempts for each container. It does not include the first, original attempt; the maximum number of total attempts will be `retries + 1`.
  name: retries
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-retry-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-container-set-retry-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-retry-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ContainerSetRetryStrategy\",\n  \"description\": \"ContainerSetRetryStrategy provides controls on how to retry a container set\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"description\": \"Duration is the time between each retry, examples values are \\\"300ms\\\", \\\"1s\\\" or \\\"5m\\\". Valid time units are \\\"ns\\\", \\\"us\\\" (or \\\"\\u00b5s\\\"), \\\"ms\\\", \\\"s\\\", \\\"m\\\", \\\"h\\\".\",\n      \"type\": \"string\"\n    },\n    \"retries\": {\n      \"description\": \"Retries is the maximum number of retry attempts for each container. It does not include the first, original attempt; the maximum number of total attempts will\
  \ be `retries + 1`.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    }\n  },\n  \"required\": [\n    \"retries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-retry-strategy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ContainerSetRetryStrategy
---
