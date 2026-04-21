---
description: MemoizationStatus is the status of this memoized node
layout: schema
name: io.argoproj.workflow.v1alpha1.MemoizationStatus
properties_list:
- description: Cache is the name of the cache that was used
  name: cacheName
  type: string
- description: Hit indicates whether this node was created from a cache entry
  name: hit
  type: boolean
- description: Key is the name of the key used for this node's cache
  name: key
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoization-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-memoization-status
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.MemoizationStatus
---
