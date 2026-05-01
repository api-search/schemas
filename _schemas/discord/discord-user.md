---
description: A user in Discord represents a person or bot account with a unique identity, username, avatar, and various account properties.
layout: schema
name: Discord User
properties_list:
- description: User ID (Snowflake)
  name: id
  type: string
- description: The user's username, not unique across the platform
  name: username
  type: string
- description: The user's Discord tag (legacy, 0 for migrated users)
  name: discriminator
  type: string
- description: The user's display name
  name: global_name
  type:
  - string
  - 'null'
- description: The user's avatar hash
  name: avatar
  type:
  - string
  - 'null'
- description: Whether the user belongs to an OAuth2 application
  name: bot
  type: boolean
- description: Whether the user is an official Discord System user
  name: system
  type: boolean
- description: Whether the user has two factor enabled
  name: mfa_enabled
  type: boolean
- description: The user's banner hash
  name: banner
  type:
  - string
  - 'null'
- description: The user's banner color as an integer
  name: accent_color
  type:
  - integer
  - 'null'
- description: The user's chosen language option
  name: locale
  type: string
- description: Whether the email on this account has been verified
  name: verified
  type: boolean
- description: The user's email
  name: email
  type:
  - string
  - 'null'
- description: The flags on a user's account
  name: flags
  type: integer
- description: The type of Nitro subscription
  name: premium_type
  type: integer
- description: The public flags on a user's account
  name: public_flags
  type: integer
- description: Data for the user's avatar decoration
  name: avatar_decoration_data
  type:
  - object
  - 'null'
provider_name: Discord
provider_slug: discord
schema_file: json-schema/discord-user-schema.json
slug: discord-user
source_filename: discord-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://discord.com/developers/schemas/discord/user.json\",\n  \"title\": \"Discord User\",\n  \"description\": \"A user in Discord represents a person or bot account with a unique identity, username, avatar, and various account properties.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"username\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User ID (Snowflake)\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The user's username, not unique across the platform\"\n    },\n    \"discriminator\": {\n      \"type\": \"string\",\n      \"description\": \"The user's Discord tag (legacy, 0 for migrated users)\"\n    },\n    \"global_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's display name\"\n    },\n    \"avatar\": {\n      \"type\"\
  : [\"string\", \"null\"],\n      \"description\": \"The user's avatar hash\"\n    },\n    \"bot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user belongs to an OAuth2 application\"\n    },\n    \"system\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is an official Discord System user\"\n    },\n    \"mfa_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has two factor enabled\"\n    },\n    \"banner\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user's banner hash\"\n    },\n    \"accent_color\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The user's banner color as an integer\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The user's chosen language option\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email on this account has been verified\"\n    },\n\
  \    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The user's email\"\n    },\n    \"flags\": {\n      \"type\": \"integer\",\n      \"description\": \"The flags on a user's account\"\n    },\n    \"premium_type\": {\n      \"type\": \"integer\",\n      \"description\": \"The type of Nitro subscription\",\n      \"enum\": [0, 1, 2, 3]\n    },\n    \"public_flags\": {\n      \"type\": \"integer\",\n      \"description\": \"The public flags on a user's account\"\n    },\n    \"avatar_decoration_data\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Data for the user's avatar decoration\",\n      \"properties\": {\n        \"asset\": {\n          \"type\": \"string\"\n        },\n        \"sku_id\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/json-schema/discord-user-schema.json
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
title: Discord User
---
