---
description: v1alpha1SyncStrategyApply schema from Argo CD API
layout: schema
name: v1alpha1SyncStrategyApply
properties_list:
- description: Force indicates whether or not to supply the --force flag to `kubectl apply`. The --force flag deletes and re-create the resource, when PATCH encounters conflict and has retried for 5 times.
  name: force
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-strategy-apply-schema.json
slug: argo-cd-v1alpha1-sync-strategy-apply
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-apply-schema.json\",\n  \"title\": \"v1alpha1SyncStrategyApply\",\n  \"description\": \"v1alpha1SyncStrategyApply schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"force\": {\n      \"description\": \"Force indicates whether or not to supply the --force flag to `kubectl apply`.\\nThe --force flag deletes and re-create the resource, when PATCH encounters conflict and has\\nretried for 5 times.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-strategy-apply-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncStrategyApply
---
