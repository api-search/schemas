---
description: Backoff is a backoff strategy to use within retryStrategy
layout: schema
name: io.argoproj.workflow.v1alpha1.Backoff
properties_list:
- description: Cap is a limit on revised values of the duration parameter. If a multiplication by the factor parameter would make the duration exceed the cap then the duration is set to the cap
  name: cap
  type: string
- description: Duration is the amount to back off. Default unit is seconds, but could also be a duration (e.g. "2m", "1h")
  name: duration
  type: string
- description: Factor is a factor to multiply the base duration after each failed retry
  name: factor
  type: object
- description: MaxDuration is the maximum amount of time allowed for a workflow in the backoff strategy. It is important to note that if the workflow template includes activeDeadlineSeconds, the pod's deadline is in
  name: maxDuration
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-backoff-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-backoff
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Backoff
---
