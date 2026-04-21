---
description: A null or empty node selector term matches no objects. The requirements of them are ANDed. The TopologySelectorTerm type implements a subset of the NodeSelectorTerm.
layout: schema
name: io.k8s.api.core.v1.NodeSelectorTerm
properties_list:
- description: A list of node selector requirements by node's labels.
  name: matchExpressions
  type: array
- description: A list of node selector requirements by node's fields.
  name: matchFields
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-term-schema.json
slug: argo-workflows-io-k8s-api-core-v1-node-selector-term
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NodeSelectorTerm
---
