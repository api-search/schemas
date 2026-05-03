---
description: Represents a video on Twitch, including VODs (archives of past streams), highlights, and uploads.
layout: schema
name: Twitch Video
properties_list:
- description: Unique identifier for the video
  name: id
  type: string
- description: ID of the stream the video was recorded from (null for uploads)
  name: stream_id
  type:
  - string
  - 'null'
- description: ID of the user who owns the video
  name: user_id
  type: string
- description: Login name of the user who owns the video
  name: user_login
  type: string
- description: Display name of the user who owns the video
  name: user_name
  type: string
- description: Title of the video
  name: title
  type: string
- description: Description of the video
  name: description
  type: string
- description: UTC timestamp when the video was created
  name: created_at
  type: string
- description: UTC timestamp when the video was published
  name: published_at
  type: string
- description: URL to view the video on Twitch
  name: url
  type: string
- description: URL template for the video thumbnail
  name: thumbnail_url
  type: string
- description: Visibility of the video
  name: viewable
  type: string
- description: Number of times the video has been viewed
  name: view_count
  type: integer
- description: Language of the video
  name: language
  type: string
- description: Type of video
  name: type
  type: string
- description: Duration of the video in ISO 8601 format (e.g., 3h21m10s)
  name: duration
  type: string
- description: Segments of the video that are muted
  name: muted_segments
  type:
  - array
  - 'null'
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-video-schema.json
slug: twitch-video
source_filename: twitch-video-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/video.json\",\n  \"title\": \"Twitch Video\",\n  \"description\": \"Represents a video on Twitch, including VODs (archives of past streams), highlights, and uploads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the video\"\n    },\n    \"stream_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the stream the video was recorded from (null for uploads)\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who owns the video\"\n    },\n    \"user_login\": {\n      \"type\": \"string\",\n      \"description\": \"Login name of the user who owns the video\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who owns the video\"\n    },\n\
  \    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the video\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the video\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp when the video was created\"\n    },\n    \"published_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp when the video was published\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view the video on Twitch\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL template for the video thumbnail\"\n    },\n    \"viewable\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"Visibility of the video\"\n    },\n \
  \   \"view_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of times the video has been viewed\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the video\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"upload\", \"archive\", \"highlight\"],\n      \"description\": \"Type of video\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"Duration of the video in ISO 8601 format (e.g., 3h21m10s)\"\n    },\n    \"muted_segments\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"type\": \"integer\",\n            \"description\": \"Duration of the muted segment in seconds\"\n          },\n          \"offset\": {\n            \"type\": \"integer\",\n            \"description\": \"Offset in the video where the muted segment begins\
  \ in seconds\"\n          }\n        }\n      },\n      \"description\": \"Segments of the video that are muted\"\n    }\n  },\n  \"required\": [\"id\", \"user_id\", \"user_login\", \"user_name\", \"title\", \"created_at\", \"published_at\", \"url\", \"thumbnail_url\", \"viewable\", \"view_count\", \"language\", \"type\", \"duration\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-video-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch Video
---
