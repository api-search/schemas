---
description: A label selector requirement is a selector that contains values, a key, and an operator that relates the key and values.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelectorRequirement
properties_list:
- description: key is the label key that the selector applies to.
  name: key
  type: string
- description: operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist.
  name: operator
  type: string
- description: values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replac
  name: values
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-requirement-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-requirement
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelectorRequirement
---
