---
description: A Restream channel representing a connected destination streaming platform account.
layout: schema
name: Channel
properties_list:
- description: Unique channel identifier
  name: id
  type: integer
- description: ID of the associated streaming platform (e.g., 1=Twitch, 5=YouTube)
  name: streamingPlatformId
  type: integer
- description: Embedded player URL for the channel
  name: embedUrl
  type: string
- description: Channel URL on the destination platform
  name: url
  type: string
- description: Platform-specific channel identifier (username, channel ID, etc.)
  name: identifier
  type: string
- description: Human-readable channel display name
  name: displayName
  type: string
- description: Whether the channel is currently active and will receive the stream
  name: active
  type: boolean
provider_name: Restream
provider_slug: restream
schema_file: json-schema/restream-channel-schema.json
slug: restream-channel
source_filename: restream-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.restream.io/schemas/channel\",\n  \"title\": \"Channel\",\n  \"description\": \"A Restream channel representing a connected destination streaming platform account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique channel identifier\"\n    },\n    \"streamingPlatformId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the associated streaming platform (e.g., 1=Twitch, 5=YouTube)\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Embedded player URL for the channel\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Channel URL on the destination platform\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Platform-specific channel identifier\
  \ (username, channel ID, etc.)\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable channel display name\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is currently active and will receive the stream\"\n    }\n  },\n  \"required\": [\"id\", \"streamingPlatformId\", \"active\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/json-schema/restream-channel-schema.json
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
title: Channel
---
