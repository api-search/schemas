---
description: Represents a Twitch user account, including profile information, broadcaster type, and account metadata.
layout: schema
name: Twitch User
properties_list:
- description: Unique identifier for the user
  name: id
  type: string
- description: User's login name (lowercase)
  name: login
  type: string
- description: User's display name
  name: display_name
  type: string
- description: User's site-wide role
  name: type
  type: string
- description: User's broadcaster type
  name: broadcaster_type
  type: string
- description: User's profile description
  name: description
  type: string
- description: URL of the user's profile image
  name: profile_image_url
  type: string
- description: URL of the user's offline image
  name: offline_image_url
  type: string
- description: User's email address (requires user:read:email scope)
  name: email
  type: string
- description: UTC timestamp when the account was created
  name: created_at
  type: string
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-user-schema.json
slug: twitch-user
source_filename: twitch-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/user.json\",\n  \"title\": \"Twitch User\",\n  \"description\": \"Represents a Twitch user account, including profile information, broadcaster type, and account metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"User's login name (lowercase)\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"User's display name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"admin\", \"global_mod\", \"staff\", \"\"],\n      \"description\": \"User's site-wide role\"\n    },\n    \"broadcaster_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"affiliate\", \"partner\", \"\"],\n      \"description\": \"User's broadcaster\
  \ type\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User's profile description\"\n    },\n    \"profile_image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's profile image\"\n    },\n    \"offline_image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's offline image\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User's email address (requires user:read:email scope)\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp when the account was created\"\n    }\n  },\n  \"required\": [\"id\", \"login\", \"display_name\", \"type\", \"broadcaster_type\", \"description\", \"profile_image_url\", \"offline_image_url\", \"created_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-user-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch User
---
