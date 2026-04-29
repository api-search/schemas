---
description: List Container Versions Response.
layout: schema
name: ListContainerVersionsResponse
properties_list:
- description: All container version headers of a GTM Container.
  name: containerVersionHeader
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-container-versions-response-schema.json
slug: google-tag-manager-v2-list-container-versions-response
source_filename: google-tag-manager-v2-list-container-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListContainerVersionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List Container Versions Response.\",\n  \"properties\": {\n    \"containerVersionHeader\": {\n      \"type\": \"array\",\n      \"description\": \"All container version headers of a GTM Container.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-container-versions-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListContainerVersionsResponse
---
