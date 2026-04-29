---
description: Basic details about a live broadcast including its title, description, and scheduled start and end times.
layout: schema
name: LiveBroadcastSnippet
properties_list:
- description: The date and time that the broadcast was added to YouTube's live broadcast schedule.
  name: publishedAt
  type: string
- description: The ID of the channel to which this broadcast is affiliated.
  name: channelId
  type: string
- description: The broadcast's title. The title is a required field when inserting a broadcast.
  name: title
  type: string
- description: The broadcast's description.
  name: description
  type: string
- description: A map of thumbnail images associated with the broadcast.
  name: thumbnails
  type: object
- description: The date and time that the broadcast is scheduled to begin.
  name: scheduledStartTime
  type: string
- description: The date and time that the broadcast is scheduled to end.
  name: scheduledEndTime
  type: string
- description: The date and time that the broadcast actually started.
  name: actualStartTime
  type: string
- description: The date and time that the broadcast actually ended.
  name: actualEndTime
  type: string
- description: The live chat ID associated with the broadcast.
  name: liveChatId
  type: string
- description: Indicates whether this broadcast is the default broadcast.
  name: isDefaultBroadcast
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-broadcast-snippet-schema.json
slug: youtube-live-live-broadcast-snippet
source_filename: youtube-live-live-broadcast-snippet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Basic details about a live broadcast including its title, description, and scheduled start and end times.\",\n  \"properties\": {\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the broadcast was added to YouTube's live broadcast schedule.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the channel to which this broadcast is affiliated.\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The broadcast's title. The title is a required field when inserting a broadcast.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The broadcast's description.\",\n      \"example\": \"A sample description for this resource.\"\
  \n    },\n    \"thumbnails\": {\n      \"type\": \"object\",\n      \"description\": \"A map of thumbnail images associated with the broadcast.\",\n      \"example\": \"example_value\"\n    },\n    \"scheduledStartTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the broadcast is scheduled to begin.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"scheduledEndTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the broadcast is scheduled to end.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"actualStartTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the broadcast actually started.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"actualEndTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the broadcast\
  \ actually ended.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"liveChatId\": {\n      \"type\": \"string\",\n      \"description\": \"The live chat ID associated with the broadcast.\",\n      \"example\": \"500123\"\n    },\n    \"isDefaultBroadcast\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this broadcast is the default broadcast.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveBroadcastSnippet\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-broadcast-snippet-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveBroadcastSnippet
---
