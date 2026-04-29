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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-node-affinity-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.NodeAffinity\",\n  \"description\": \"Node affinity is a group of node affinity scheduling rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"preferredDuringSchedulingIgnoredDuringExecution\": {\n      \"description\": \"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \\\"weight\\\
  \" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.PreferredSchedulingTerm\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"requiredDuringSchedulingIgnoredDuringExecution\": {\n      \"description\": \"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to an update), the system may or may not try to eventually evict the pod from its node.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.NodeSelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-node-affinity-schema.json
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
