---
description: Defines the Google Tag Manager Account access permissions.
layout: schema
name: AccountAccess
properties_list:
- description: Whether the user has no access, user access, or admin access to the account.
  name: permission
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-account-access-schema.json
slug: google-tag-manager-v2-account-access
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountAccess\",\n  \"type\": \"object\",\n  \"description\": \"Defines the Google Tag Manager Account access permissions.\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the user has no access, user access, or admin access to the account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-account-access-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: AccountAccess
---
