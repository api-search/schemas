---
description: sync.UpdateSyncLimitRequest schema from Argo Workflows API
layout: schema
name: sync.UpdateSyncLimitRequest
properties_list:
- description: ''
  name: cmName
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: limit
  type: integer
- description: ''
  name: namespace
  type: string
- description: ''
  name: type
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-sync-update-sync-limit-request-schema.json
slug: argo-workflows-sync-update-sync-limit-request
source_filename: argo-workflows-sync-update-sync-limit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sync-update-sync-limit-request-schema.json\",\n  \"title\": \"sync.UpdateSyncLimitRequest\",\n  \"description\": \"sync.UpdateSyncLimitRequest schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmName\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"$ref\": \"#/definitions/sync.SyncConfigType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-sync-update-sync-limit-request-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: sync.UpdateSyncLimitRequest
---
