---
description: A node selector represents the union of the results of one or more label queries over a set of nodes; that is, it represents the OR of the selectors represented by the node selector terms.
layout: schema
name: io.k8s.api.core.v1.NodeSelector
properties_list:
- description: Required. A list of node selector terms. The terms are ORed.
  name: nodeSelectorTerms
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-node-selector
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NodeSelector
---
