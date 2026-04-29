---
description: A liveChatModerator resource identifies a user who has moderator privileges in a YouTube live chat.
layout: schema
name: LiveChatModerator
properties_list:
- description: Identifies the API resource's type. Value is youtube#liveChatModerator.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube assigns to uniquely identify the moderator.
  name: id
  type: string
- description: The snippet object contains basic details about the moderator.
  name: snippet
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-chat-moderator-schema.json
slug: youtube-live-live-chat-moderator
source_filename: youtube-live-live-chat-moderator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A liveChatModerator resource identifies a user who has moderator privileges in a YouTube live chat.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#liveChatModerator.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube assigns to uniquely identify the moderator.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet object contains basic details about the moderator.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"liveChatId\": {\n          \"type\": \"string\",\n          \"\
  description\": \"The liveChatId is the live chat id for this moderator resource.\"\n        },\n        \"moderatorDetails\": {\n          \"type\": \"object\",\n          \"description\": \"Details about the moderator.\",\n          \"properties\": {\n            \"channelId\": {\n              \"type\": \"string\",\n              \"description\": \"The YouTube channel ID of the moderator.\"\n            },\n            \"channelUrl\": {\n              \"type\": \"string\",\n              \"description\": \"The channel URL of the moderator.\"\n            },\n            \"displayName\": {\n              \"type\": \"string\",\n              \"description\": \"The channel's display name.\"\n            },\n            \"profileImageUrl\": {\n              \"type\": \"string\",\n              \"description\": \"The channel's avatar URL.\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"LiveChatModerator\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-chat-moderator-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveChatModerator
---
