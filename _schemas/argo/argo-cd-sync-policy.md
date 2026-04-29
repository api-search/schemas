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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-sync-policy-schema.json\",\n  \"title\": \"SyncPolicy\",\n  \"description\": \"Policy controlling how and when the application is synchronized.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"automated\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for automatic synchronization.\",\n      \"properties\": {\n        \"prune\": {\n          \"type\": \"boolean\",\n          \"description\": \"Automatically delete resources removed from the source.\",\n          \"default\": false\n        },\n        \"selfHeal\": {\n          \"type\": \"boolean\",\n          \"description\": \"Automatically sync when live state drifts from desired state.\",\n          \"default\": false\n        },\n        \"allowEmpty\": {\n          \"type\": \"boolean\",\n          \"description\": \"\
  Allows apps to have an empty source.\",\n          \"default\": false\n        }\n      }\n    },\n    \"syncOptions\": {\n      \"type\": \"array\",\n      \"description\": \"List of sync option flags (e.g., CreateNamespace=true, PrunePropagationPolicy=foreground).\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"retry\": {\n      \"type\": \"object\",\n      \"description\": \"Retry configuration for failed sync operations.\",\n      \"properties\": {\n        \"limit\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum number of retry attempts. -1 for unlimited.\"\n        },\n        \"backoff\": {\n          \"type\": \"object\",\n          \"description\": \"Backoff strategy for retries.\",\n          \"properties\": {\n            \"duration\": {\n              \"type\": \"string\",\n              \"description\": \"Initial retry backoff duration.\"\n            },\n            \"factor\": {\n\
  \              \"type\": \"integer\",\n              \"format\": \"int64\",\n              \"description\": \"Multiplicative factor applied to duration on each retry.\"\n            },\n            \"maxDuration\": {\n              \"type\": \"string\",\n              \"description\": \"Maximum duration between retries.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-sync-policy-schema.json
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
