---
description: List user permissions response.
layout: schema
name: ListUserPermissionsResponse
properties_list:
- description: All GTM UserPermissions of a GTM Account.
  name: userPermission
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-user-permissions-response-schema.json
slug: google-tag-manager-v2-list-user-permissions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListUserPermissionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List user permissions response.\",\n  \"properties\": {\n    \"userPermission\": {\n      \"type\": \"array\",\n      \"description\": \"All GTM UserPermissions of a GTM Account.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-user-permissions-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListUserPermissionsResponse
---
