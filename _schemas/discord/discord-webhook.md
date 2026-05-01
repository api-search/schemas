---
description: A webhook in Discord provides a way to post messages to channels without requiring a bot user or authentication, supporting incoming, channel follower, and application webhook types.
layout: schema
name: Discord Webhook
properties_list:
- description: Webhook ID (Snowflake)
  name: id
  type: string
- description: 'Type of webhook: 1=Incoming, 2=Channel Follower, 3=Application'
  name: type
  type: integer
- description: Guild ID this webhook is for
  name: guild_id
  type:
  - string
  - 'null'
- description: Channel ID this webhook is for
  name: channel_id
  type:
  - string
  - 'null'
- description: User that created this webhook
  name: user
  type: object
- description: Default name of the webhook
  name: name
  type:
  - string
  - 'null'
- description: Default user avatar hash of the webhook
  name: avatar
  type:
  - string
  - 'null'
- description: Secure token of the webhook (Incoming type only)
  name: token
  type: string
- description: Bot/OAuth2 application that created this webhook
  name: application_id
  type:
  - string
  - 'null'
- description: Guild of the channel that this webhook is following (Channel Follower only)
  name: source_guild
  type: object
- description: Channel that this webhook is following (Channel Follower only)
  name: source_channel
  type: object
- description: URL used for executing the webhook
  name: url
  type: string
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-webhook-schema.json
slug: discord-webhook
source_filename: discord-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/webhook.json\",\n  \"title\": \"Discord Webhook\",\n  \"description\": \"A webhook in Discord provides a way to post messages to channels without requiring a bot user or authentication, supporting incoming, channel follower, and application webhook types.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook ID (Snowflake)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"type\": {\n      \"type\": \"integer\",\n      \"description\": \"Type of webhook: 1=Incoming, 2=Channel Follower, 3=Application\",\n      \"enum\": [1, 2, 3]\n    },\n    \"guild_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Guild ID this webhook is for\"\n    },\n    \"channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"Channel ID this webhook is for\"\n    },\n    \"user\": {\n      \"$ref\": \"discord-user-schema.json\",\n      \"description\": \"User that created this webhook\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default name of the webhook\"\n    },\n    \"avatar\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Default user avatar hash of the webhook\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Secure token of the webhook (Incoming type only)\"\n    },\n    \"application_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Bot/OAuth2 application that created this webhook\"\n    },\n    \"source_guild\": {\n      \"type\": \"object\",\n      \"description\": \"Guild of the channel that this webhook is following (Channel Follower only)\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n       \
  \ \"icon\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"source_channel\": {\n      \"type\": \"object\",\n      \"description\": \"Channel that this webhook is following (Channel Follower only)\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL used for executing the webhook\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-webhook-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord Webhook
---
