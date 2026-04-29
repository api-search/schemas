---
description: v1alpha1SyncPolicyAutomated schema from Argo CD API
layout: schema
name: v1alpha1SyncPolicyAutomated
properties_list:
- description: ''
  name: allowEmpty
  type: boolean
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: prune
  type: boolean
- description: ''
  name: selfHeal
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-policy-automated-schema.json
slug: argo-cd-v1alpha1-sync-policy-automated
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-policy-automated-schema.json\",\n  \"title\": \"v1alpha1SyncPolicyAutomated\",\n  \"description\": \"v1alpha1SyncPolicyAutomated schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowEmpty\": {\n      \"type\": \"boolean\",\n      \"title\": \"AllowEmpty allows apps have zero live resources (default: false)\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"title\": \"Enable allows apps to explicitly control automated sync\"\n    },\n    \"prune\": {\n      \"type\": \"boolean\",\n      \"title\": \"Prune specifies whether to delete resources from the cluster that are not found in the sources anymore as part of automated sync (default: false)\"\n    },\n    \"selfHeal\": {\n      \"type\": \"boolean\",\n      \"title\": \"SelfHeal specifies\
  \ whether to revert resources back to their desired state upon modification in the cluster (default: false)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-policy-automated-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncPolicyAutomated
---
