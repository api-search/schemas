---
description: v1alpha1SyncStrategy schema from Argo CD API
layout: schema
name: v1alpha1SyncStrategy
properties_list:
- description: ''
  name: apply
  type: object
- description: ''
  name: hook
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-strategy-schema.json
slug: argo-cd-v1alpha1-sync-strategy
source_filename: argo-cd-v1alpha1-sync-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-schema.json\",\n  \"title\": \"v1alpha1SyncStrategy\",\n  \"description\": \"v1alpha1SyncStrategy schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apply\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStrategyApply\"\n    },\n    \"hook\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncStrategyHook\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncStrategy
---
