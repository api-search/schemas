---
description: SyncSource specifies a location from which hydrated manifests may be synced. RepoURL is assumed based on the associated DrySource config in the SourceHydrator.
layout: schema
name: v1alpha1SyncSource
properties_list:
- description: Path is a directory path within the git repository where hydrated manifests should be committed to and synced from. The Path should never point to the root of the repo. If hydrateTo is set, this is ju
  name: path
  type: string
- description: TargetBranch is the branch from which hydrated manifests will be synced. If HydrateTo is not set, this is also the branch to which hydrated manifests are committed.
  name: targetBranch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-source-schema.json
slug: argo-cd-v1alpha1-sync-source
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncSource
---
