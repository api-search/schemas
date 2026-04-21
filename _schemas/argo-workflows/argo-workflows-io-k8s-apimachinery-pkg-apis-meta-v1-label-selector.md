---
description: A label selector is a label query over a set of resources. The result of matchLabels and matchExpressions are ANDed. An empty label selector matches all objects. A null label selector matches no objects.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector
properties_list:
- description: matchExpressions is a list of label selector requirements. The requirements are ANDed.
  name: matchExpressions
  type: array
- description: matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is "key", the operator is "In", and the values a
  name: matchLabels
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector
---
