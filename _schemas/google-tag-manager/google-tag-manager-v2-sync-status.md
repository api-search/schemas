---
description: The status of a workspace after syncing.
layout: schema
name: SyncStatus
properties_list:
- description: Synchornization operation detected a merge conflict.
  name: mergeConflict
  type: boolean
- description: An error occurred during the sync operation.
  name: syncError
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-sync-status-schema.json
slug: google-tag-manager-v2-sync-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SyncStatus\",\n  \"type\": \"object\",\n  \"description\": \"The status of a workspace after syncing.\",\n  \"properties\": {\n    \"mergeConflict\": {\n      \"type\": \"boolean\",\n      \"description\": \"Synchornization operation detected a merge conflict.\"\n    },\n    \"syncError\": {\n      \"type\": \"boolean\",\n      \"description\": \"An error occurred during the sync operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-sync-status-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: SyncStatus
---
