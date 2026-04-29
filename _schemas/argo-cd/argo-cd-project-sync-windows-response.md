---
description: projectSyncWindowsResponse schema from Argo CD API
layout: schema
name: projectSyncWindowsResponse
properties_list:
- description: ''
  name: windows
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-project-sync-windows-response-schema.json
slug: argo-cd-project-sync-windows-response
source_filename: argo-cd-project-sync-windows-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-sync-windows-response-schema.json\",\n  \"title\": \"projectSyncWindowsResponse\",\n  \"description\": \"projectSyncWindowsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"windows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1SyncWindow\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-sync-windows-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: projectSyncWindowsResponse
---
