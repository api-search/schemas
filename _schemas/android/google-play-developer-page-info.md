---
description: Pagination information for list responses.
layout: schema
name: PageInfo
properties_list:
- description: Total number of results available.
  name: totalResults
  type: integer
- description: Maximum number of results per page.
  name: resultPerPage
  type: integer
- description: Index of the first result returned.
  name: startIndex
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-page-info-schema.json
slug: google-play-developer-page-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageInfo\",\n  \"type\": \"object\",\n  \"description\": \"Pagination information for list responses.\",\n  \"properties\": {\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results available.\"\n    },\n    \"resultPerPage\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results per page.\"\n    },\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of the first result returned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-page-info-schema.json
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
title: PageInfo
---
