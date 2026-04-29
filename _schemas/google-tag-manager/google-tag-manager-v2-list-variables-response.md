---
description: List Variables Response.
layout: schema
name: ListVariablesResponse
properties_list:
- description: All GTM Variables of a GTM Container Workspace.
  name: variable
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-variables-response-schema.json
slug: google-tag-manager-v2-list-variables-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListVariablesResponse\",\n  \"type\": \"object\",\n  \"description\": \"List Variables Response.\",\n  \"properties\": {\n    \"variable\": {\n      \"type\": \"array\",\n      \"description\": \"All GTM Variables of a GTM Container Workspace.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-variables-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListVariablesResponse
---
