---
description: List Workspaces Response.
layout: schema
name: ListWorkspacesResponse
properties_list:
- description: All Workspaces of a GTM Container.
  name: workspace
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-workspaces-response-schema.json
slug: google-tag-manager-v2-list-workspaces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListWorkspacesResponse\",\n  \"type\": \"object\",\n  \"description\": \"List Workspaces Response.\",\n  \"properties\": {\n    \"workspace\": {\n      \"type\": \"array\",\n      \"description\": \"All Workspaces of a GTM Container.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-workspaces-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListWorkspacesResponse
---
