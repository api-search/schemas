---
description: ApplicationSetSpec represents a class of application set state.
layout: schema
name: v1alpha1ApplicationSetSpec
properties_list:
- description: 'ApplyNestedSelectors enables selectors defined within the generators of two level-nested matrix or merge generators. Deprecated: This field is ignored, and the behavior is always enabled. The field wi'
  name: applyNestedSelectors
  type: boolean
- description: ''
  name: generators
  type: array
- description: ''
  name: goTemplate
  type: boolean
- description: ''
  name: goTemplateOptions
  type: array
- description: ''
  name: ignoreApplicationDifferences
  type: array
- description: ''
  name: preservedFields
  type: object
- description: ''
  name: strategy
  type: object
- description: ''
  name: syncPolicy
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: templatePatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-spec-schema.json
slug: argo-cd-v1alpha1-application-set-spec
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetSpec
---
