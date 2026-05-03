---
description: Represents an active live stream on Twitch, including broadcaster information, game category, viewer count, and stream metadata.
layout: schema
name: Twitch Stream
properties_list:
- description: Unique identifier for the stream
  name: id
  type: string
- description: ID of the user who is streaming
  name: user_id
  type: string
- description: Login name of the user who is streaming
  name: user_login
  type: string
- description: Display name of the user who is streaming
  name: user_name
  type: string
- description: ID of the game/category being played
  name: game_id
  type: string
- description: Name of the game/category being played
  name: game_name
  type: string
- description: Stream type (live or empty string if offline)
  name: type
  type: string
- description: Title of the stream
  name: title
  type: string
- description: Number of current viewers
  name: viewer_count
  type: integer
- description: UTC timestamp when the stream started
  name: started_at
  type: string
- description: Language of the stream (BCP 47)
  name: language
  type: string
- description: URL template for the stream thumbnail
  name: thumbnail_url
  type: string
- description: Tags applied to the stream
  name: tags
  type: array
- description: Whether the stream is marked as mature content
  name: is_mature
  type: boolean
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-stream-schema.json
slug: twitch-stream
source_filename: twitch-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/stream.json\",\n  \"title\": \"Twitch Stream\",\n  \"description\": \"Represents an active live stream on Twitch, including broadcaster information, game category, viewer count, and stream metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the stream\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who is streaming\"\n    },\n    \"user_login\": {\n      \"type\": \"string\",\n      \"description\": \"Login name of the user who is streaming\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who is streaming\"\n    },\n    \"game_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the game/category being played\"\n    },\n    \"game_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the game/category being played\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"live\", \"\"],\n      \"description\": \"Stream type (live or empty string if offline)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the stream\"\n    },\n    \"viewer_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of current viewers\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp when the stream started\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the stream (BCP 47)\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL template for the stream thumbnail\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n    \
  \  \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags applied to the stream\"\n    },\n    \"is_mature\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the stream is marked as mature content\"\n    }\n  },\n  \"required\": [\"id\", \"user_id\", \"user_login\", \"user_name\", \"type\", \"title\", \"viewer_count\", \"started_at\", \"language\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-stream-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch Stream
---
