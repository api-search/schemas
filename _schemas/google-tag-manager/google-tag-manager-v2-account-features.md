---
description: Read-only account feature set.
layout: schema
name: AccountFeatures
properties_list:
- description: Whether this account has user permissions management enabled.
  name: supportUserPermissions
  type: boolean
- description: Whether this account supports multiple containers.
  name: supportMultipleContainers
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-account-features-schema.json
slug: google-tag-manager-v2-account-features
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountFeatures\",\n  \"type\": \"object\",\n  \"description\": \"Read-only account feature set.\",\n  \"properties\": {\n    \"supportUserPermissions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this account has user permissions management enabled.\"\n    },\n    \"supportMultipleContainers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this account supports multiple containers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-account-features-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: AccountFeatures
---
