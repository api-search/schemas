---
description: Policy controlling how and when the application is synchronized.
layout: schema
name: SyncPolicy
properties_list:
- description: Configuration for automatic synchronization.
  name: automated
  type: object
- description: List of sync option flags (e.g., CreateNamespace=true, PrunePropagationPolicy=foreground).
  name: syncOptions
  type: array
- description: Retry configuration for failed sync operations.
  name: retry
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-sync-policy-schema.json
slug: argo-cd-sync-policy
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: SyncPolicy
---
