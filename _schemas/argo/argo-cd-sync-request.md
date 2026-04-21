---
description: Request body for triggering an application sync operation.
layout: schema
name: SyncRequest
properties_list:
- description: Specific Git revision to sync to. Defaults to the current target revision.
  name: revision
  type: string
- description: Preview sync without applying changes.
  name: dryRun
  type: boolean
- description: Delete resources no longer defined in the source.
  name: prune
  type: boolean
- description: Sync strategy configuration.
  name: strategy
  type: object
- description: Specific resources to sync (partial sync).
  name: resources
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-sync-request-schema.json
slug: argo-cd-sync-request
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: SyncRequest
---
