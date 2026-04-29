---
description: A Slack user object representing a workspace member with their profile, roles, and settings.
layout: schema
name: User
properties_list:
- description: The unique identifier for this user.
  name: id
  type: string
- description: The workspace team ID this user belongs to.
  name: team_id
  type: string
- description: The user's username.
  name: name
  type: string
- description: Whether the user has been deactivated.
  name: deleted
  type: boolean
- description: A hex color code used in certain client displays for this user.
  name: color
  type: string
- description: The user's real name.
  name: real_name
  type: string
- description: The user's timezone identifier (e.g., "America/Los_Angeles").
  name: tz
  type: string
- description: Descriptive label for the user's timezone.
  name: tz_label
  type: string
- description: The user's timezone offset from UTC in seconds.
  name: tz_offset
  type: integer
- description: The user's profile information.
  name: profile
  type: object
- description: Whether the user is a workspace admin.
  name: is_admin
  type: boolean
- description: Whether the user is a workspace owner.
  name: is_owner
  type: boolean
- description: Whether the user is the primary workspace owner.
  name: is_primary_owner
  type: boolean
- description: Whether the user is a guest with single-channel access.
  name: is_restricted
  type: boolean
- description: Whether the user is a single-channel guest.
  name: is_ultra_restricted
  type: boolean
- description: Whether the user is a bot.
  name: is_bot
  type: boolean
- description: Whether the user is an app user.
  name: is_app_user
  type: boolean
- description: Unix timestamp of when the user was last updated.
  name: updated
  type: integer
- description: Whether the user has two-factor authentication enabled.
  name: has_2fa
  type: boolean
- description: IETF language code for the user. Only included when specifically requested.
  name: locale
  type: string
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-user-schema.json
slug: slack-web-user
source_filename: slack-web-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A Slack user object representing a workspace member with their profile, roles, and settings.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this user.\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace team ID this user belongs to.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user's username.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has been deactivated.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"A hex color code used in certain client displays for this user.\"\n    },\n    \"real_name\": {\n      \"type\": \"string\",\n      \"description\": \"The user's real name.\"\n    },\n\
  \    \"tz\": {\n      \"type\": \"string\",\n      \"description\": \"The user's timezone identifier (e.g., \\\"America/Los_Angeles\\\").\"\n    },\n    \"tz_label\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive label for the user's timezone.\"\n    },\n    \"tz_offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The user's timezone offset from UTC in seconds.\"\n    },\n    \"profile\": {\n      \"type\": \"object\",\n      \"description\": \"The user's profile information.\"\n    },\n    \"is_admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a workspace admin.\"\n    },\n    \"is_owner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a workspace owner.\"\n    },\n    \"is_primary_owner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is the primary workspace owner.\"\n    },\n    \"is_restricted\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the user is a guest with single-channel access.\"\n    },\n    \"is_ultra_restricted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a single-channel guest.\"\n    },\n    \"is_bot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a bot.\"\n    },\n    \"is_app_user\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is an app user.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the user was last updated.\"\n    },\n    \"has_2fa\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has two-factor authentication enabled.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"IETF language code for the user. Only included when specifically requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-user-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: User
---
