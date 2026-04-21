---
description: Node affinity is a group of node affinity scheduling rules.
layout: schema
name: io.k8s.api.core.v1.NodeAffinity
properties_list:
- description: 'The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that '
  name: preferredDuringSchedulingIgnoredDuringExecution
  type: array
- description: If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met a
  name: requiredDuringSchedulingIgnoredDuringExecution
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-node-affinity-schema.json
slug: argo-workflows-io-k8s-api-core-v1-node-affinity
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NodeAffinity
---
