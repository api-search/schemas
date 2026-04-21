---
description: The weights of all of the matched WeightedPodAffinityTerm fields are added per-node to find the most preferred node(s)
layout: schema
name: io.k8s.api.core.v1.WeightedPodAffinityTerm
properties_list:
- description: Required. A pod affinity term, associated with the corresponding weight.
  name: podAffinityTerm
  type: object
- description: weight associated with matching the corresponding podAffinityTerm, in the range 1-100.
  name: weight
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term-schema.json
slug: argo-workflows-io-k8s-api-core-v1-weighted-pod-affinity-term
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.WeightedPodAffinityTerm
---
