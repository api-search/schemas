---
description: applicationApplicationSyncWindowsResponse schema from Argo CD API
layout: schema
name: applicationApplicationSyncWindowsResponse
properties_list:
- description: ''
  name: activeWindows
  type: array
- description: ''
  name: assignedWindows
  type: array
- description: ''
  name: canSync
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-application-sync-windows-response-schema.json
slug: argo-cd-application-application-sync-windows-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-sync-windows-response-schema.json\",\n  \"title\": \"applicationApplicationSyncWindowsResponse\",\n  \"description\": \"applicationApplicationSyncWindowsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeWindows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationApplicationSyncWindow\"\n      }\n    },\n    \"assignedWindows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationApplicationSyncWindow\"\n      }\n    },\n    \"canSync\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-sync-windows-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationApplicationSyncWindowsResponse
---
