---
description: A list of video category resources matching the request criteria.
layout: schema
name: VideoCategoryListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#videoCategoryListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: A list of video categories that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-category-list-response-schema.json
slug: youtube-data-video-category-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of video category resources matching the request criteria.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#videoCategoryListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of video categories that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A videoCategory resource identifies a category that has been or could be associated with uploaded videos.\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's\
  \ type. Value is youtube#videoCategory.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the video category.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the video category.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"channelId\": {\n                \"type\": \"string\",\n                \"description\": \"The YouTube channel that created the video category.\"\n              },\n              \"title\": {\n                \"type\": \"string\",\n    \
  \            \"description\": \"The video category's title.\"\n              },\n              \"assignable\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether videos can be associated with the category.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoCategoryListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-category-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoCategoryListResponse
---
