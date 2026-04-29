---
description: Statistics about the video such as the number of times the video has been viewed or liked.
layout: schema
name: VideoStatistics
properties_list:
- description: The number of times the video has been viewed.
  name: viewCount
  type: string
- description: The number of users who have indicated that they liked the video.
  name: likeCount
  type: string
- description: The number of users who have indicated that they disliked the video.
  name: dislikeCount
  type: string
- description: The number of users who have added the video to their favorites list.
  name: favoriteCount
  type: string
- description: The number of comments for the video.
  name: commentCount
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-statistics-schema.json
slug: youtube-data-video-statistics
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Statistics about the video such as the number of times the video has been viewed or liked.\",\n  \"properties\": {\n    \"viewCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of times the video has been viewed.\",\n      \"example\": 42\n    },\n    \"likeCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of users who have indicated that they liked the video.\",\n      \"example\": 42\n    },\n    \"dislikeCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of users who have indicated that they disliked the video.\",\n      \"example\": 42\n    },\n    \"favoriteCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of users who have added the video to their favorites list.\",\n      \"example\": 42\n    },\n    \"commentCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of comments for the video.\",\n\
  \      \"example\": 42\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoStatistics\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-statistics-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoStatistics
---
