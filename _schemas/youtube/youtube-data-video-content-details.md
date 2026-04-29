---
description: Information about the video content, including the length of the video and an indication of whether captions are available.
layout: schema
name: VideoContentDetails
properties_list:
- description: The length of the video in ISO 8601 format.
  name: duration
  type: string
- description: Indicates whether the video is available in 3D or in 2D.
  name: dimension
  type: string
- description: Indicates whether the video is available in high definition or standard definition.
  name: definition
  type: string
- description: Indicates whether captions are available for the video.
  name: caption
  type: string
- description: Indicates whether the video represents licensed content, which means that the content has been claimed by a YouTube content partner.
  name: licensedContent
  type: boolean
- description: Specifies the ratings that the video received under various rating schemes.
  name: contentRating
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-content-details-schema.json
slug: youtube-data-video-content-details
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Information about the video content, including the length of the video and an indication of whether captions are available.\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The length of the video in ISO 8601 format.\",\n      \"example\": \"example_value\"\n    },\n    \"dimension\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the video is available in 3D or in 2D.\",\n      \"example\": \"example_value\"\n    },\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the video is available in high definition or standard definition.\",\n      \"example\": \"hd\",\n      \"enum\": [\n        \"hd\",\n        \"sd\"\n      ]\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether captions are available for the video.\",\n      \"example\": \"false\",\n      \"enum\"\
  : [\n        \"false\",\n        \"true\"\n      ]\n    },\n    \"licensedContent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the video represents licensed content, which means that the content has been claimed by a YouTube content partner.\",\n      \"example\": true\n    },\n    \"contentRating\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the ratings that the video received under various rating schemes.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoContentDetails\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-content-details-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoContentDetails
---
