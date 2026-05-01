---
description: An emoji in Discord, either a custom guild emoji or a standard Unicode emoji used in messages, reactions, and components.
layout: schema
name: Discord Emoji
properties_list:
- description: Emoji ID (null for standard Unicode emojis)
  name: id
  type:
  - string
  - 'null'
- description: Emoji name (can be null for reaction emoji objects)
  name: name
  type:
  - string
  - 'null'
- description: Roles allowed to use this emoji
  name: roles
  type: array
- description: User that created this emoji
  name: user
  type: object
- description: Whether this emoji must be wrapped in colons
  name: require_colons
  type: boolean
- description: Whether this emoji is managed by an integration
  name: managed
  type: boolean
- description: Whether this emoji is animated
  name: animated
  type: boolean
- description: Whether this emoji can be used (may be false due to server boost loss)
  name: available
  type: boolean
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-emoji-schema.json
slug: discord-emoji
source_filename: discord-emoji-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/emoji.json\",\n  \"title\": \"Discord Emoji\",\n  \"description\": \"An emoji in Discord, either a custom guild emoji or a standard Unicode emoji used in messages, reactions, and components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Emoji ID (null for standard Unicode emojis)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Emoji name (can be null for reaction emoji objects)\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"description\": \"Roles allowed to use this emoji\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"user\": {\n      \"$ref\": \"discord-user-schema.json\",\n      \"description\": \"User that created this emoji\"\n    },\n\
  \    \"require_colons\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this emoji must be wrapped in colons\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this emoji is managed by an integration\"\n    },\n    \"animated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this emoji is animated\"\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this emoji can be used (may be false due to server boost loss)\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-emoji-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord Emoji
---
