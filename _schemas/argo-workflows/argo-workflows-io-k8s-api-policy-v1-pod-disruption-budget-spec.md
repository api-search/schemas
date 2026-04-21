---
description: PodDisruptionBudgetSpec is a description of a PodDisruptionBudget.
layout: schema
name: io.k8s.api.policy.v1.PodDisruptionBudgetSpec
properties_list:
- description: An eviction is allowed if at most "maxUnavailable" pods selected by "selector" are unavailable after the eviction, i.e. even in absence of the evicted pod. For example, one can prevent all voluntary e
  name: maxUnavailable
  type: object
- description: An eviction is allowed if at least "minAvailable" pods selected by "selector" will still be available after the eviction, i.e. even in the absence of the evicted pod. So for example you can prevent al
  name: minAvailable
  type: object
- description: Label query over pods whose evictions are managed by the disruption budget. A null selector will match no pods, while an empty ({}) selector will select all pods within the namespace.
  name: selector
  type: object
- description: 'UnhealthyPodEvictionPolicy defines the criteria for when unhealthy pods should be considered for eviction. Current implementation considers healthy pods, as pods that have status.conditions item with '
  name: unhealthyPodEvictionPolicy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-policy-v1-pod-disruption-budget-spec-schema.json
slug: argo-workflows-io-k8s-api-policy-v1-pod-disruption-budget-spec
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.policy.v1.PodDisruptionBudgetSpec
---
