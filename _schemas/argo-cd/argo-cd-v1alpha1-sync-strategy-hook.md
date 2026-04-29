---
description: SyncStrategyHook will perform a sync using hooks annotations. If no hook annotation is specified falls back to `kubectl apply`.
layout: schema
name: v1alpha1SyncStrategyHook
properties_list:
- description: ''
  name: syncStrategyApply
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-strategy-hook-schema.json
slug: argo-cd-v1alpha1-sync-strategy-hook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-hook-schema.json\",\n  \"title\": \"v1alpha1SyncStrategyHook\",\n  \"description\": \"SyncStrategyHook will perform a sync using hooks annotations.\\nIf no hook annotation is specified falls back to `kubectl apply`.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"syncStrategyApply\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStrategyApply\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-hook-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncStrategyHook
---
