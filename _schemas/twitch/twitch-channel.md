---
description: Represents a Twitch channel with its current configuration including title, game, language, tags, and content classification.
layout: schema
name: Twitch Channel
properties_list:
- description: Unique identifier for the broadcaster
  name: broadcaster_id
  type: string
- description: Broadcaster's login name
  name: broadcaster_login
  type: string
- description: Broadcaster's display name
  name: broadcaster_name
  type: string
- description: Language of the channel (BCP 47)
  name: broadcaster_language
  type: string
- description: ID of the current game/category
  name: game_id
  type: string
- description: Name of the current game/category
  name: game_name
  type: string
- description: Title of the stream
  name: title
  type: string
- description: Stream delay in seconds (partners only)
  name: delay
  type: integer
- description: Tags applied to the channel
  name: tags
  type: array
- description: Content classification labels applied to the channel
  name: content_classification_labels
  type: array
- description: Whether the channel has branded content
  name: is_branded_content
  type: boolean
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-channel-schema.json
slug: twitch-channel
source_filename: twitch-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/channel.json\",\n  \"title\": \"Twitch Channel\",\n  \"description\": \"Represents a Twitch channel with its current configuration including title, game, language, tags, and content classification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"broadcaster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the broadcaster\"\n    },\n    \"broadcaster_login\": {\n      \"type\": \"string\",\n      \"description\": \"Broadcaster's login name\"\n    },\n    \"broadcaster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Broadcaster's display name\"\n    },\n    \"broadcaster_language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the channel (BCP 47)\"\n    },\n    \"game_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the current game/category\"\n    },\n \
  \   \"game_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the current game/category\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the stream\"\n    },\n    \"delay\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Stream delay in seconds (partners only)\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags applied to the channel\"\n    },\n    \"content_classification_labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Content classification labels applied to the channel\"\n    },\n    \"is_branded_content\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel has branded content\"\n    }\n  },\n  \"required\": [\"broadcaster_id\", \"broadcaster_login\", \"broadcaster_name\", \"broadcaster_language\"\
  , \"game_id\", \"game_name\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-channel-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch Channel
---
