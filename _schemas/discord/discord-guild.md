---
description: A guild (server) in Discord represents an isolated collection of users and channels, and is often referred to as a server in the UI.
layout: schema
name: Discord Guild
properties_list:
- description: Guild ID (Snowflake)
  name: id
  type: string
- description: Guild name (2-100 characters)
  name: name
  type: string
- description: Icon hash
  name: icon
  type:
  - string
  - 'null'
- description: Icon hash, returned in template object
  name: icon_hash
  type:
  - string
  - 'null'
- description: Splash hash
  name: splash
  type:
  - string
  - 'null'
- description: Discovery splash hash
  name: discovery_splash
  type:
  - string
  - 'null'
- description: True if the user is the owner of the guild
  name: owner
  type: boolean
- description: ID of the guild owner
  name: owner_id
  type: string
- description: Total permissions for the user in the guild
  name: permissions
  type: string
- description: ID of AFK channel
  name: afk_channel_id
  type:
  - string
  - 'null'
- description: AFK timeout in seconds
  name: afk_timeout
  type: integer
- description: Whether the server widget is enabled
  name: widget_enabled
  type: boolean
- description: Channel ID that the widget generates an invite to
  name: widget_channel_id
  type:
  - string
  - 'null'
- description: Verification level required for the guild
  name: verification_level
  type: integer
- description: Default message notification level
  name: default_message_notifications
  type: integer
- description: Explicit content filter level
  name: explicit_content_filter
  type: integer
- description: Roles in the guild
  name: roles
  type: array
- description: Custom guild emojis
  name: emojis
  type: array
- description: Enabled guild features
  name: features
  type: array
- description: Required MFA level for the guild
  name: mfa_level
  type: integer
- description: System channel ID for system messages
  name: system_channel_id
  type:
  - string
  - 'null'
- description: System channel flags
  name: system_channel_flags
  type: integer
- description: Channel ID for community rules
  name: rules_channel_id
  type:
  - string
  - 'null'
- description: Maximum number of presences for the guild
  name: max_presences
  type:
  - integer
  - 'null'
- description: Maximum number of members for the guild
  name: max_members
  type: integer
- description: Vanity URL code for the guild
  name: vanity_url_code
  type:
  - string
  - 'null'
- description: Description of the guild
  name: description
  type:
  - string
  - 'null'
- description: Banner hash
  name: banner
  type:
  - string
  - 'null'
- description: Server boost level
  name: premium_tier
  type: integer
- description: Number of boosts this guild currently has
  name: premium_subscription_count
  type: integer
- description: Preferred locale of a community guild
  name: preferred_locale
  type: string
- description: Channel ID for moderator community updates
  name: public_updates_channel_id
  type:
  - string
  - 'null'
- description: Maximum users in a video channel
  name: max_video_channel_users
  type: integer
- description: Maximum users in a stage video channel
  name: max_stage_video_channel_users
  type: integer
- description: Approximate number of members in the guild
  name: approximate_member_count
  type: integer
- description: Approximate number of online members
  name: approximate_presence_count
  type: integer
- description: Guild NSFW level
  name: nsfw_level
  type: integer
- description: Whether the guild has the boost progress bar enabled
  name: premium_progress_bar_enabled
  type: boolean
- description: Channel ID for safety alerts
  name: safety_alerts_channel_id
  type:
  - string
  - 'null'
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-guild-schema.json
slug: discord-guild
source_filename: discord-guild-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/guild.json\",\n  \"title\": \"Discord Guild\",\n  \"description\": \"A guild (server) in Discord represents an isolated collection of users and channels, and is often referred to as a server in the UI.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Guild ID (Snowflake)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Guild name (2-100 characters)\",\n      \"minLength\": 2,\n      \"maxLength\": 100\n    },\n    \"icon\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Icon hash\"\n    },\n    \"icon_hash\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Icon hash, returned in template object\"\n    },\n    \"splash\": {\n      \"type\"\
  : [\"string\", \"null\"],\n      \"description\": \"Splash hash\"\n    },\n    \"discovery_splash\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Discovery splash hash\"\n    },\n    \"owner\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the user is the owner of the guild\"\n    },\n    \"owner_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the guild owner\"\n    },\n    \"permissions\": {\n      \"type\": \"string\",\n      \"description\": \"Total permissions for the user in the guild\"\n    },\n    \"afk_channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of AFK channel\"\n    },\n    \"afk_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"AFK timeout in seconds\",\n      \"enum\": [60, 300, 900, 1800, 3600]\n    },\n    \"widget_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the server widget is enabled\"\n    },\n    \"widget_channel_id\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel ID that the widget generates an invite to\"\n    },\n    \"verification_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Verification level required for the guild\",\n      \"enum\": [0, 1, 2, 3, 4]\n    },\n    \"default_message_notifications\": {\n      \"type\": \"integer\",\n      \"description\": \"Default message notification level\",\n      \"enum\": [0, 1]\n    },\n    \"explicit_content_filter\": {\n      \"type\": \"integer\",\n      \"description\": \"Explicit content filter level\",\n      \"enum\": [0, 1, 2]\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"description\": \"Roles in the guild\",\n      \"items\": {\n        \"$ref\": \"discord-role-schema.json\"\n      }\n    },\n    \"emojis\": {\n      \"type\": \"array\",\n      \"description\": \"Custom guild emojis\",\n      \"items\": {\n        \"$ref\": \"discord-emoji-schema.json\"\n      }\n    },\n    \"\
  features\": {\n      \"type\": \"array\",\n      \"description\": \"Enabled guild features\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"mfa_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Required MFA level for the guild\",\n      \"enum\": [0, 1]\n    },\n    \"system_channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"System channel ID for system messages\"\n    },\n    \"system_channel_flags\": {\n      \"type\": \"integer\",\n      \"description\": \"System channel flags\"\n    },\n    \"rules_channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel ID for community rules\"\n    },\n    \"max_presences\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Maximum number of presences for the guild\"\n    },\n    \"max_members\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of members for the guild\"\n    },\n    \"vanity_url_code\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Vanity URL code for the guild\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of the guild\"\n    },\n    \"banner\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Banner hash\"\n    },\n    \"premium_tier\": {\n      \"type\": \"integer\",\n      \"description\": \"Server boost level\",\n      \"enum\": [0, 1, 2, 3]\n    },\n    \"premium_subscription_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of boosts this guild currently has\"\n    },\n    \"preferred_locale\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred locale of a community guild\"\n    },\n    \"public_updates_channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel ID for moderator community updates\"\n    },\n    \"max_video_channel_users\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Maximum users in a video channel\"\n    },\n    \"max_stage_video_channel_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum users in a stage video channel\"\n    },\n    \"approximate_member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of members in the guild\"\n    },\n    \"approximate_presence_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of online members\"\n    },\n    \"nsfw_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Guild NSFW level\",\n      \"enum\": [0, 1, 2, 3]\n    },\n    \"premium_progress_bar_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the guild has the boost progress bar enabled\"\n    },\n    \"safety_alerts_channel_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel ID for safety alerts\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-guild-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord Guild
---
