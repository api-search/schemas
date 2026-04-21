---
description: HydrateTo specifies a location to which hydrated manifests should be pushed as a "staging area" before being moved to the SyncSource. The RepoURL and Path are assumed based on the associated SyncSource config in the SourceHydrator.
layout: schema
name: v1alpha1HydrateTo
properties_list:
- description: ''
  name: targetBranch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-hydrate-to-schema.json
slug: argo-cd-v1alpha1-hydrate-to
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HydrateTo
---
