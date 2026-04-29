---
description: v1alpha1SyncOperationResult schema from Argo CD API
layout: schema
name: v1alpha1SyncOperationResult
properties_list:
- description: ''
  name: managedNamespaceMetadata
  type: object
- description: ''
  name: resources
  type: array
- description: ''
  name: revision
  type: string
- description: ''
  name: revisions
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: sources
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-operation-result-schema.json
slug: argo-cd-v1alpha1-sync-operation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-operation-result-schema.json\",\n  \"title\": \"v1alpha1SyncOperationResult\",\n  \"description\": \"v1alpha1SyncOperationResult schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"managedNamespaceMetadata\": {\n      \"$ref\": \"#/definitions/v1alpha1ManagedNamespaceMetadata\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"title\": \"Resources contains a list of sync result items for each individual resource in a sync operation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceResult\"\n      }\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"title\": \"Revision holds the revision this sync operation was performed to\"\n    },\n    \"revisions\": {\n      \"type\": \"array\",\n      \"title\": \"Revisions\
  \ holds the revision this sync operation was performed for respective indexed source in sources field\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"title\": \"Source records the application source information of the sync, used for comparing auto-sync\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-operation-result-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncOperationResult
---
