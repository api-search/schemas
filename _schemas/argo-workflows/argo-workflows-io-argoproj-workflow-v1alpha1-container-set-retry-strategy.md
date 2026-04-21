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
