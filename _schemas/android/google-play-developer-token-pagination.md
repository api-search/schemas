---
description: Token-based pagination for large result sets.
layout: schema
name: TokenPagination
properties_list:
- description: Token to retrieve the next page of results.
  name: nextPageToken
  type: string
- description: Token to retrieve the previous page of results.
  name: previousPageToken
  type: string
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-token-pagination-schema.json
slug: google-play-developer-token-pagination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenPagination\",\n  \"type\": \"object\",\n  \"description\": \"Token-based pagination for large result sets.\",\n  \"properties\": {\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token to retrieve the next page of results.\"\n    },\n    \"previousPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token to retrieve the previous page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-token-pagination-schema.json
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
title: TokenPagination
---
