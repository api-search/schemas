---
description: ResourceIgnoreDifferences contains resource filter and list of json paths which should be ignored during comparison with live state.
layout: schema
name: v1alpha1ResourceIgnoreDifferences
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: jqPathExpressions
  type: array
- description: ''
  name: jsonPointers
  type: array
- description: ''
  name: kind
  type: string
- description: ''
  name: managedFieldsManagers
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-ignore-differences-schema.json
slug: argo-cd-v1alpha1-resource-ignore-differences
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceIgnoreDifferences
---
