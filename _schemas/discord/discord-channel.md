---
description: A channel in Discord represents a text, voice, category, thread, forum, or other communication medium within a guild or direct message.
layout: schema
name: Discord Channel
properties_list:
- description: Channel ID (Snowflake)
  name: id
  type: string
- description: Type of channel
  name: type
  type: integer
- description: ID of the guild the channel belongs to
  name: guild_id
  type: string
- description: Sorting position of the channel
  name: position
  type: integer
- description: Explicit permission overwrites for members and roles
  name: permission_overwrites
  type: array
- description: Channel name (1-100 characters)
  name: name
  type:
  - string
  - 'null'
- description: Channel topic (0-4096 characters for forum/media, 0-1024 otherwise)
  name: topic
  type:
  - string
  - 'null'
- description: Whether the channel is NSFW
  name: nsfw
  type: boolean
- description: ID of the last message sent in this channel
  name: last_message_id
  type:
  - string
  - 'null'
- description: Bitrate of the voice or stage channel
  name: bitrate
  type: integer
- description: User limit of the voice or stage channel
  name: user_limit
  type: integer
- description: Slowmode rate limit in seconds (0-21600)
  name: rate_limit_per_user
  type: integer
- description: Recipients of the DM
  name: recipients
  type: array
- description: Icon hash of the group DM
  name: icon
  type:
  - string
  - 'null'
- description: ID of the creator of the group DM or thread
  name: owner_id
  type: string
- description: ID of the parent category or channel
  name: parent_id
  type:
  - string
  - 'null'
- description: When the last pinned message was pinned
  name: last_pin_timestamp
  type:
  - string
  - 'null'
- description: Voice region ID for the voice channel
  name: rtc_region
  type:
  - string
  - 'null'
- description: Video quality mode of the voice channel
  name: video_quality_mode
  type: integer
- description: Approximate count of messages in a thread
  name: message_count
  type: integer
- description: Approximate count of users in a thread
  name: member_count
  type: integer
- description: ''
  name: thread_metadata
  type: object
- description: Default auto archive duration for new threads
  name: default_auto_archive_duration
  type: integer
- description: Channel flags combined as a bitfield
  name: flags
  type: integer
- description: Total messages ever sent in a thread
  name: total_message_sent
  type: integer
- description: Default slowmode for new threads in this channel
  name: default_thread_rate_limit_per_user
  type: integer
- description: Default sort order for forum/media channels
  name: default_sort_order
  type:
  - integer
  - 'null'
- description: Default layout for forum channels
  name: default_forum_layout
  type: integer
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-channel-schema.json
slug: discord-channel
source_filename: discord-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/channel.json\",\n  \"title\": \"Discord Channel\",\n  \"description\": \"A channel in Discord represents a text, voice, category, thread, forum, or other communication medium within a guild or direct message.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Channel ID (Snowflake)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"type\": {\n      \"type\": \"integer\",\n      \"description\": \"Type of channel\",\n      \"enum\": [0, 1, 2, 3, 4, 5, 10, 11, 12, 13, 14, 15, 16]\n    },\n    \"guild_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the guild the channel belongs to\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Sorting position of the channel\"\n    },\n    \"permission_overwrites\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Explicit permission overwrites for members and roles\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PermissionOverwrite\"\n      }\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel name (1-100 characters)\",\n      \"maxLength\": 100\n    },\n    \"topic\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Channel topic (0-4096 characters for forum/media, 0-1024 otherwise)\",\n      \"maxLength\": 4096\n    },\n    \"nsfw\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is NSFW\"\n    },\n    \"last_message_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the last message sent in this channel\"\n    },\n    \"bitrate\": {\n      \"type\": \"integer\",\n      \"description\": \"Bitrate of the voice or stage channel\"\n    },\n    \"user_limit\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"User limit of the voice or stage channel\"\n    },\n    \"rate_limit_per_user\": {\n      \"type\": \"integer\",\n      \"description\": \"Slowmode rate limit in seconds (0-21600)\",\n      \"minimum\": 0,\n      \"maximum\": 21600\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"Recipients of the DM\",\n      \"items\": {\n        \"$ref\": \"discord-user-schema.json\"\n      }\n    },\n    \"icon\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Icon hash of the group DM\"\n    },\n    \"owner_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the creator of the group DM or thread\"\n    },\n    \"parent_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent category or channel\"\n    },\n    \"last_pin_timestamp\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the last pinned message was pinned\"\n    },\n\
  \    \"rtc_region\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Voice region ID for the voice channel\"\n    },\n    \"video_quality_mode\": {\n      \"type\": \"integer\",\n      \"description\": \"Video quality mode of the voice channel\",\n      \"enum\": [1, 2]\n    },\n    \"message_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate count of messages in a thread\"\n    },\n    \"member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate count of users in a thread\"\n    },\n    \"thread_metadata\": {\n      \"$ref\": \"#/$defs/ThreadMetadata\"\n    },\n    \"default_auto_archive_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Default auto archive duration for new threads\",\n      \"enum\": [60, 1440, 4320, 10080]\n    },\n    \"flags\": {\n      \"type\": \"integer\",\n      \"description\": \"Channel flags combined as a bitfield\"\n    },\n    \"total_message_sent\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Total messages ever sent in a thread\"\n    },\n    \"default_thread_rate_limit_per_user\": {\n      \"type\": \"integer\",\n      \"description\": \"Default slowmode for new threads in this channel\"\n    },\n    \"default_sort_order\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Default sort order for forum/media channels\"\n    },\n    \"default_forum_layout\": {\n      \"type\": \"integer\",\n      \"description\": \"Default layout for forum channels\"\n    }\n  },\n  \"$defs\": {\n    \"PermissionOverwrite\": {\n      \"type\": \"object\",\n      \"description\": \"A permission overwrite for a role or member\",\n      \"required\": [\"id\", \"type\", \"allow\", \"deny\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Role or user ID\"\n        },\n        \"type\": {\n          \"type\": \"integer\",\n          \"description\": \"0 for role, 1 for member\"\
  ,\n          \"enum\": [0, 1]\n        },\n        \"allow\": {\n          \"type\": \"string\",\n          \"description\": \"Permission bit set for allowed permissions\"\n        },\n        \"deny\": {\n          \"type\": \"string\",\n          \"description\": \"Permission bit set for denied permissions\"\n        }\n      }\n    },\n    \"ThreadMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for a thread channel\",\n      \"properties\": {\n        \"archived\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the thread is archived\"\n        },\n        \"auto_archive_duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Duration in minutes to auto-archive after inactivity\"\n        },\n        \"archive_timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the thread's archive status was last changed\"\n        },\n      \
  \  \"locked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the thread is locked\"\n        },\n        \"invitable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether non-moderators can add users to the thread\"\n        },\n        \"create_timestamp\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the thread was created\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-channel-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord Channel
---
