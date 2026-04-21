---
description: A node selector requirement is a selector that contains values, a key, and an operator that relates the key and values.
layout: schema
name: io.k8s.api.core.v1.NodeSelectorRequirement
properties_list:
- description: The label key that the selector applies to.
  name: key
  type: string
- description: Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt.
  name: operator
  type: string
- description: An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, t
  name: values
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-requirement-schema.json
slug: argo-workflows-io-k8s-api-core-v1-node-selector-requirement
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NodeSelectorRequirement
---
