---
description: Represents a clip created from a Twitch live stream or VOD, including metadata about the broadcaster, creator, and source video.
layout: schema
name: Twitch Clip
properties_list:
- description: Unique identifier for the clip
  name: id
  type: string
- description: URL to view the clip on Twitch
  name: url
  type: string
- description: URL to embed the clip
  name: embed_url
  type: string
- description: ID of the broadcaster whose channel the clip was created on
  name: broadcaster_id
  type: string
- description: Display name of the broadcaster
  name: broadcaster_name
  type: string
- description: ID of the user who created the clip
  name: creator_id
  type: string
- description: Display name of the clip creator
  name: creator_name
  type: string
- description: ID of the video the clip was created from
  name: video_id
  type: string
- description: ID of the game/category during clip creation
  name: game_id
  type: string
- description: Language of the stream when the clip was created
  name: language
  type: string
- description: Title of the clip
  name: title
  type: string
- description: Number of times the clip has been viewed
  name: view_count
  type: integer
- description: UTC timestamp when the clip was created
  name: created_at
  type: string
- description: URL of the clip's thumbnail image
  name: thumbnail_url
  type: string
- description: Duration of the clip in seconds
  name: duration
  type: number
- description: Offset in the VOD where the clip starts (null if VOD is unavailable)
  name: vod_offset
  type:
  - integer
  - 'null'
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-clip-schema.json
slug: twitch-clip
source_filename: twitch-clip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/clip.json\",\n  \"title\": \"Twitch Clip\",\n  \"description\": \"Represents a clip created from a Twitch live stream or VOD, including metadata about the broadcaster, creator, and source video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the clip\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view the clip on Twitch\"\n    },\n    \"embed_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to embed the clip\"\n    },\n    \"broadcaster_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the broadcaster whose channel the clip was created on\"\n    },\n    \"broadcaster_name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Display name of the broadcaster\"\n    },\n    \"creator_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the clip\"\n    },\n    \"creator_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the clip creator\"\n    },\n    \"video_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the video the clip was created from\"\n    },\n    \"game_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the game/category during clip creation\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the stream when the clip was created\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the clip\"\n    },\n    \"view_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of times the clip has been viewed\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"UTC timestamp when the clip was created\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the clip's thumbnail image\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Duration of the clip in seconds\"\n    },\n    \"vod_offset\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Offset in the VOD where the clip starts (null if VOD is unavailable)\"\n    }\n  },\n  \"required\": [\"id\", \"url\", \"embed_url\", \"broadcaster_id\", \"broadcaster_name\", \"creator_id\", \"creator_name\", \"title\", \"view_count\", \"created_at\", \"thumbnail_url\", \"duration\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-clip-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch Clip
---
