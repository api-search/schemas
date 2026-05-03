---
description: A group channel for messaging between users in Sendbird.
layout: schema
name: Sendbird Group Channel
properties_list:
- description: Unique URL identifier for the channel.
  name: channel_url
  type: string
- description: Display name of the group channel.
  name: name
  type: string
- description: URL for the channel cover image.
  name: cover_url
  type: string
- description: Total number of members in the channel.
  name: member_count
  type: integer
- description: Number of members who have joined (not left) the channel.
  name: joined_member_count
  type: integer
- description: Number of unread messages for the requesting user.
  name: unread_message_count
  type: integer
- description: Whether this is a distinct channel — only one channel can exist for a given set of members.
  name: is_distinct
  type: boolean
- description: Unix timestamp (milliseconds) when the channel was created.
  name: created_at
  type: integer
- description: Custom data string associated with the channel.
  name: data
  type: string
- description: Custom type for channel categorization.
  name: custom_type
  type: string
provider_name: Sendbird
provider_slug: sendbird
schema_file: json-schema/sendbird-group-channel-schema.json
slug: sendbird-group-channel
source_filename: sendbird-group-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sendbird/json-schema/sendbird-group-channel-schema.json\",\n  \"title\": \"Sendbird Group Channel\",\n  \"description\": \"A group channel for messaging between users in Sendbird.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel_url\": {\n      \"type\": \"string\",\n      \"description\": \"Unique URL identifier for the channel.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the group channel.\"\n    },\n    \"cover_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the channel cover image.\"\n    },\n    \"member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of members in the channel.\"\n    },\n    \"joined_member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members who have joined (not\
  \ left) the channel.\"\n    },\n    \"unread_message_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unread messages for the requesting user.\"\n    },\n    \"is_distinct\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a distinct channel — only one channel can exist for a given set of members.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (milliseconds) when the channel was created.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Custom data string associated with the channel.\"\n    },\n    \"custom_type\": {\n      \"type\": \"string\",\n      \"description\": \"Custom type for channel categorization.\"\n    }\n  },\n  \"required\": [\"channel_url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/json-schema/sendbird-group-channel-schema.json
tags: []
title: Sendbird Group Channel
---
