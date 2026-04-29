---
description: v1alpha1SyncStatus schema from Argo CD API
layout: schema
name: v1alpha1SyncStatus
properties_list:
- description: ''
  name: comparedTo
  type: object
- description: ''
  name: revision
  type: string
- description: ''
  name: revisions
  type: array
- description: ''
  name: status
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-status-schema.json
slug: argo-cd-v1alpha1-sync-status
source_filename: argo-cd-v1alpha1-sync-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-status-schema.json\",\n  \"title\": \"v1alpha1SyncStatus\",\n  \"description\": \"v1alpha1SyncStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparedTo\": {\n      \"$ref\": \"#/definitions/v1alpha1ComparedTo\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"title\": \"Revision contains information about the revision the comparison has been performed to\"\n    },\n    \"revisions\": {\n      \"type\": \"array\",\n      \"title\": \"Revisions contains information about the revisions of multiple sources the comparison has been performed to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status is the sync state of the comparison\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncStatus
---
