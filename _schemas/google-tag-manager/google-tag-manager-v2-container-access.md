---
description: Defines the Google Tag Manager Container access permissions.
layout: schema
name: ContainerAccess
properties_list:
- description: GTM Container ID.
  name: containerId
  type: string
- description: List of Container permissions. Valid values include noAccess, read, edit, approve, and publish.
  name: permission
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-container-access-schema.json
slug: google-tag-manager-v2-container-access
source_filename: google-tag-manager-v2-container-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerAccess\",\n  \"type\": \"object\",\n  \"description\": \"Defines the Google Tag Manager Container access permissions.\",\n  \"properties\": {\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Container ID.\"\n    },\n    \"permission\": {\n      \"type\": \"string\",\n      \"description\": \"List of Container permissions. Valid values include noAccess, read, edit, approve, and publish.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-container-access-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ContainerAccess
---
