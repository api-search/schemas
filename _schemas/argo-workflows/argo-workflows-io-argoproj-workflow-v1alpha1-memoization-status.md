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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoization-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.MemoizationStatus\",\n  \"description\": \"MemoizationStatus is the status of this memoized node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cacheName\": {\n      \"description\": \"Cache is the name of the cache that was used\",\n      \"type\": \"string\"\n    },\n    \"hit\": {\n      \"description\": \"Hit indicates whether this node was created from a cache entry\",\n      \"type\": \"boolean\"\n    },\n    \"key\": {\n      \"description\": \"Key is the name of the key used for this node's cache\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"hit\",\n    \"key\",\n    \"cacheName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoization-status-schema.json
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
