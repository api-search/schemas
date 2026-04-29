---
description: The changes and conflicts in a workspace, providing information about which entities have been modified and any merge conflicts.
layout: schema
name: GetWorkspaceStatusResponse
properties_list:
- description: Entities that have been changed in the workspace.
  name: workspaceChange
  type: array
- description: The merge conflict after sync.
  name: mergeConflict
  type: array
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-get-workspace-status-response-schema.json
slug: google-tag-manager-v2-get-workspace-status-response
source_filename: google-tag-manager-v2-get-workspace-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetWorkspaceStatusResponse\",\n  \"type\": \"object\",\n  \"description\": \"The changes and conflicts in a workspace, providing information about which entities have been modified and any merge conflicts.\",\n  \"properties\": {\n    \"workspaceChange\": {\n      \"type\": \"array\",\n      \"description\": \"Entities that have been changed in the workspace.\"\n    },\n    \"mergeConflict\": {\n      \"type\": \"array\",\n      \"description\": \"The merge conflict after sync.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-get-workspace-status-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: GetWorkspaceStatusResponse
---
