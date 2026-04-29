---
description: Represents a Google Tag Manager Workspace. A workspace is an isolated editing environment within a container where changes to tags, triggers, and variables can be made and tested before being published.
layout: schema
name: Workspace
properties_list:
- description: GTM Workspace's API relative path.
  name: path
  type: string
- description: GTM Account ID.
  name: accountId
  type: string
- description: GTM Container ID.
  name: containerId
  type: string
- description: The Workspace ID uniquely identifies the GTM Workspace.
  name: workspaceId
  type: string
- description: Workspace display name.
  name: name
  type: string
- description: Workspace description.
  name: description
  type: string
- description: The fingerprint of the GTM Workspace as computed at storage time. This value is recomputed whenever the workspace is modified.
  name: fingerprint
  type: string
- description: Auto-generated link to the tag manager UI.
  name: tagManagerUrl
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-workspace-schema.json
slug: google-tag-manager-v2-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workspace\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Google Tag Manager Workspace. A workspace is an isolated editing environment within a container where changes to tags, triggers, and variables can be made and tested before being published.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Workspace's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Account ID.\"\n    },\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Container ID.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The Workspace ID uniquely identifies the GTM Workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workspace display name.\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Workspace description.\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The fingerprint of the GTM Workspace as computed at storage time. This value is recomputed whenever the workspace is modified.\"\n    },\n    \"tagManagerUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated link to the tag manager UI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-workspace-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: Workspace
---
