---
description: A label selector requirement is a selector that contains values, a key, and an operator that relates the key and values.
layout: schema
name: v1LabelSelectorRequirement
properties_list:
- description: key is the label key that the selector applies to.
  name: key
  type: string
- description: operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist.
  name: operator
  type: string
- description: ''
  name: values
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-label-selector-requirement-schema.json
slug: argo-cd-v1-label-selector-requirement
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1LabelSelectorRequirement
---
