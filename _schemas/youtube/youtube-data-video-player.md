---
description: Information used to play the video.
layout: schema
name: VideoPlayer
properties_list:
- description: An iframe tag that embeds a player that will play the video.
  name: embedHtml
  type: string
- description: The height of the embedded player returned in the player.embedHtml property.
  name: embedHeight
  type: number
- description: The width of the embedded player returned in the player.embedHtml property.
  name: embedWidth
  type: number
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-player-schema.json
slug: youtube-data-video-player
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Information used to play the video.\",\n  \"properties\": {\n    \"embedHtml\": {\n      \"type\": \"string\",\n      \"description\": \"An iframe tag that embeds a player that will play the video.\",\n      \"example\": \"example_value\"\n    },\n    \"embedHeight\": {\n      \"type\": \"number\",\n      \"description\": \"The height of the embedded player returned in the player.embedHtml property.\",\n      \"example\": 42.5\n    },\n    \"embedWidth\": {\n      \"type\": \"number\",\n      \"description\": \"The width of the embedded player returned in the player.embedHtml property.\",\n      \"example\": 42.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoPlayer\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-player-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoPlayer
---
