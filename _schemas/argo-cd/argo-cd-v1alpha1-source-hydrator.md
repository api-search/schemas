---
description: SourceHydrator specifies a dry "don't repeat yourself" source for manifests, a sync source from which to sync hydrated manifests, and an optional hydrateTo location to act as a "staging" aread for hydrated manifests.
layout: schema
name: v1alpha1SourceHydrator
properties_list:
- description: ''
  name: drySource
  type: object
- description: ''
  name: hydrateTo
  type: object
- description: ''
  name: syncSource
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-source-hydrator-schema.json
slug: argo-cd-v1alpha1-source-hydrator
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SourceHydrator
---
