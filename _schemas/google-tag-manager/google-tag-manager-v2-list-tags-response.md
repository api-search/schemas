---
description: List Tags Response.
layout: schema
name: ListTagsResponse
properties_list:
- description: All GTM Tags of a GTM Container Workspace.
  name: tag
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-tags-response-schema.json
slug: google-tag-manager-v2-list-tags-response
source_filename: google-tag-manager-v2-list-tags-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List Tags Response.\",\n  \"properties\": {\n    \"tag\": {\n      \"type\": \"array\",\n      \"description\": \"All GTM Tags of a GTM Container Workspace.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-tags-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListTagsResponse
---
