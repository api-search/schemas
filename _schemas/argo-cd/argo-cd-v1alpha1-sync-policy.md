---
description: v1alpha1SyncPolicy schema from Argo CD API
layout: schema
name: v1alpha1SyncPolicy
properties_list:
- description: ''
  name: automated
  type: object
- description: ''
  name: managedNamespaceMetadata
  type: object
- description: ''
  name: retry
  type: object
- description: ''
  name: syncOptions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-policy-schema.json
slug: argo-cd-v1alpha1-sync-policy
source_filename: argo-cd-v1alpha1-sync-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-policy-schema.json\",\n  \"title\": \"v1alpha1SyncPolicy\",\n  \"description\": \"v1alpha1SyncPolicy schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"automated\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncPolicyAutomated\"\n    },\n    \"managedNamespaceMetadata\": {\n      \"$ref\": \"#/definitions/v1alpha1ManagedNamespaceMetadata\"\n    },\n    \"retry\": {\n      \"$ref\": \"#/definitions/v1alpha1RetryStrategy\"\n    },\n    \"syncOptions\": {\n      \"type\": \"array\",\n      \"title\": \"Options allow you to specify whole app sync-options\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-policy-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncPolicy
---
