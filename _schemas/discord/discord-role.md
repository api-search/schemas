---
description: A role in Discord represents a set of permissions and visual attributes that can be assigned to guild members to control access and display hierarchy.
layout: schema
name: Discord Role
properties_list:
- description: Role ID (Snowflake)
  name: id
  type: string
- description: Role name
  name: name
  type: string
- description: Integer representation of hexadecimal color code
  name: color
  type: integer
- description: Whether this role is pinned in the user listing
  name: hoist
  type: boolean
- description: Role icon hash
  name: icon
  type:
  - string
  - 'null'
- description: Role unicode emoji
  name: unicode_emoji
  type:
  - string
  - 'null'
- description: Position of this role (higher = more authority)
  name: position
  type: integer
- description: Permission bit set
  name: permissions
  type: string
- description: Whether this role is managed by an integration
  name: managed
  type: boolean
- description: Whether this role is mentionable
  name: mentionable
  type: boolean
- description: ''
  name: tags
  type: object
- description: Role flags combined as a bitfield
  name: flags
  type: integer
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-role-schema.json
slug: discord-role
source_filename: discord-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/role.json\",\n  \"title\": \"Discord Role\",\n  \"description\": \"A role in Discord represents a set of permissions and visual attributes that can be assigned to guild members to control access and display hierarchy.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"color\", \"hoist\", \"position\", \"permissions\", \"managed\", \"mentionable\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Role ID (Snowflake)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Role name\",\n      \"maxLength\": 100\n    },\n    \"color\": {\n      \"type\": \"integer\",\n      \"description\": \"Integer representation of hexadecimal color code\"\n    },\n    \"hoist\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this\
  \ role is pinned in the user listing\"\n    },\n    \"icon\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Role icon hash\"\n    },\n    \"unicode_emoji\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Role unicode emoji\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Position of this role (higher = more authority)\"\n    },\n    \"permissions\": {\n      \"type\": \"string\",\n      \"description\": \"Permission bit set\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this role is managed by an integration\"\n    },\n    \"mentionable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this role is mentionable\"\n    },\n    \"tags\": {\n      \"$ref\": \"#/$defs/RoleTags\"\n    },\n    \"flags\": {\n      \"type\": \"integer\",\n      \"description\": \"Role flags combined as a bitfield\"\n    }\n  },\n  \"$defs\": {\n    \"RoleTags\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Tags indicating special properties of the role\",\n      \"properties\": {\n        \"bot_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the bot this role belongs to\"\n        },\n        \"integration_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the integration this role belongs to\"\n        },\n        \"premium_subscriber\": {\n          \"type\": \"null\",\n          \"description\": \"Whether this is the guild's Booster role (present if true)\"\n        },\n        \"subscription_listing_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of this role's subscription SKU and listing\"\n        },\n        \"available_for_purchase\": {\n          \"type\": \"null\",\n          \"description\": \"Whether this role is available for purchase (present if true)\"\n        },\n        \"guild_connections\": {\n          \"type\": \"null\",\n        \
  \  \"description\": \"Whether this role is a guild's linked role (present if true)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-role-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord Role
---
