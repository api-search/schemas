---
description: SyncOperation contains details about a sync operation.
layout: schema
name: v1alpha1SyncOperation
properties_list:
- description: ''
  name: autoHealAttemptsCount
  type: integer
- description: ''
  name: dryRun
  type: boolean
- description: ''
  name: manifests
  type: array
- description: ''
  name: prune
  type: boolean
- description: ''
  name: resources
  type: array
- description: Revision is the revision (Git) or chart version (Helm) which to sync the application to If omitted, will use the revision specified in app spec.
  name: revision
  type: string
- description: Revisions is the list of revision (Git) or chart version (Helm) which to sync each source in sources field for the application to If omitted, will use the revision specified in app spec.
  name: revisions
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: sources
  type: array
- description: ''
  name: syncOptions
  type: array
- description: ''
  name: syncStrategy
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-operation-schema.json
slug: argo-cd-v1alpha1-sync-operation
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncOperation
---
