---
description: Paging details for a list of live streaming resources.
layout: schema
name: PageInfo
properties_list:
- description: The total number of results in the result set.
  name: totalResults
  type: integer
- description: The number of results included in the API response.
  name: resultsPerPage
  type: integer
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-page-info-schema.json
slug: youtube-live-page-info
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paging details for a list of live streaming resources.\",\n  \"properties\": {\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of results in the result set.\",\n      \"example\": 42\n    },\n    \"resultsPerPage\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results included in the API response.\",\n      \"example\": 10\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageInfo\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-page-info-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: PageInfo
---
