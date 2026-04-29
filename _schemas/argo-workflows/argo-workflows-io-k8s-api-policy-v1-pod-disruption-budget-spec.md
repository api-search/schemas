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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-policy-v1-pod-disruption-budget-spec-schema.json\",\n  \"title\": \"io.k8s.api.policy.v1.PodDisruptionBudgetSpec\",\n  \"description\": \"PodDisruptionBudgetSpec is a description of a PodDisruptionBudget.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxUnavailable\": {\n      \"description\": \"An eviction is allowed if at most \\\"maxUnavailable\\\" pods selected by \\\"selector\\\" are unavailable after the eviction, i.e. even in absence of the evicted pod. For example, one can prevent all voluntary evictions by specifying 0. This is a mutually exclusive setting with \\\"minAvailable\\\".\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"minAvailable\": {\n      \"description\": \"An eviction is allowed if at least\
  \ \\\"minAvailable\\\" pods selected by \\\"selector\\\" will still be available after the eviction, i.e. even in the absence of the evicted pod.  So for example you can prevent all voluntary evictions by specifying \\\"100%\\\".\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"selector\": {\n      \"description\": \"Label query over pods whose evictions are managed by the disruption budget. A null selector will match no pods, while an empty ({}) selector will select all pods within the namespace.\",\n      \"x-kubernetes-patch-strategy\": \"replace\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector\"\n    },\n    \"unhealthyPodEvictionPolicy\": {\n      \"description\": \"UnhealthyPodEvictionPolicy defines the criteria for when unhealthy pods should be considered for eviction. Current implementation considers healthy pods, as pods that have status.conditions item with type=\\\"Ready\\\",status=\\\"\
  True\\\".\\n\\nValid policies are IfHealthyBudget and AlwaysAllow. If no policy is specified, the default behavior will be used, which corresponds to the IfHealthyBudget policy.\\n\\nIfHealthyBudget policy means that running pods (status.phase=\\\"Running\\\"), but not yet healthy can be evicted only if the guarded application is not disrupted (status.currentHealthy is at least equal to status.desiredHealthy). Healthy pods will be subject to the PDB for eviction.\\n\\nAlwaysAllow policy means that all running pods (status.phase=\\\"Running\\\"), but not yet healthy are considered disrupted and can be evicted regardless of whether the criteria in a PDB is met. This means perspective running pods of a disrupted application might not get a chance to become healthy. Healthy pods will be subject to the PDB for eviction.\\n\\nAdditional policies may be added in the future. Clients making eviction decisions should disallow eviction of unhealthy pods if they encounter an unrecognized policy in\
  \ this field.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-policy-v1-pod-disruption-budget-spec-schema.json
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
