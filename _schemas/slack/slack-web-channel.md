---
description: A Slack conversation object representing a channel, direct message, multi-person DM, or group conversation.
layout: schema
name: Channel
properties_list:
- description: The unique identifier for this conversation.
  name: id
  type: string
- description: 'The name of the channel (without the leading # sign).'
  name: name
  type: string
- description: Normalized version of the channel name.
  name: name_normalized
  type: string
- description: Whether this is a public channel.
  name: is_channel
  type: boolean
- description: Whether this is a private channel (formerly a group).
  name: is_group
  type: boolean
- description: Whether this is a direct message.
  name: is_im
  type: boolean
- description: Whether this is a multi-person direct message.
  name: is_mpim
  type: boolean
- description: Whether this is a private conversation.
  name: is_private
  type: boolean
- description: Whether the channel is archived.
  name: is_archived
  type: boolean
- description: Whether this is the
  name: is_general
  type: boolean
- description: Whether the channel is shared with another workspace.
  name: is_shared
  type: boolean
- description: Whether the channel is shared with an external organization via Slack Connect.
  name: is_ext_shared
  type: boolean
- description: Whether the channel is shared across an Enterprise Grid org.
  name: is_org_shared
  type: boolean
- description: Whether there is a pending external share invitation.
  name: is_pending_ext_shared
  type: boolean
- description: Whether the calling user is a member of this conversation.
  name: is_member
  type: boolean
- description: Whether the DM is open.
  name: is_open
  type: boolean
- description: Whether the channel is frozen.
  name: is_frozen
  type: boolean
- description: Unix timestamp of when the conversation was created.
  name: created
  type: integer
- description: User ID of the member who created this channel.
  name: creator
  type: string
- description: Unix timestamp of the last update to the conversation.
  name: updated
  type: integer
- description: Number of times the channel has been unlinked.
  name: unlinked
  type: integer
- description: The channel topic.
  name: topic
  type: object
- description: The channel purpose.
  name: purpose
  type: object
- description: A list of previous names the channel had.
  name: previous_names
  type: array
- description: The number of members in the channel. Only included when specifically requested.
  name: num_members
  type: integer
- description: IETF language code for the channel locale. Only included when specifically requested.
  name: locale
  type: string
- description: For direct messages, the user ID of the other participant.
  name: user
  type: string
- description: Array of team IDs that share this channel (for shared channels).
  name: shared_team_ids
  type: array
- description: Parent conversation ID for thread-only channels.
  name: parent_conversation
  type: string
- description: The workspace team ID.
  name: context_team_id
  type: string
- description: Additional channel properties.
  name: properties
  type: object
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-channel-schema.json
slug: slack-web-channel
source_filename: slack-web-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Channel\",\n  \"type\": \"object\",\n  \"description\": \"A Slack conversation object representing a channel, direct message, multi-person DM, or group conversation.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this conversation.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the channel (without the leading # sign).\"\n    },\n    \"name_normalized\": {\n      \"type\": \"string\",\n      \"description\": \"Normalized version of the channel name.\"\n    },\n    \"is_channel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a public channel.\"\n    },\n    \"is_group\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a private channel (formerly a group).\"\n    },\n    \"is_im\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether this is a direct message.\"\n    },\n    \"is_mpim\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a multi-person direct message.\"\n    },\n    \"is_private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a private conversation.\"\n    },\n    \"is_archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is archived.\"\n    },\n    \"is_general\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the\"\n    },\n    \"is_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared with another workspace.\"\n    },\n    \"is_ext_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared with an external organization via Slack Connect.\"\n    },\n    \"is_org_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared across an Enterprise\
  \ Grid org.\"\n    },\n    \"is_pending_ext_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there is a pending external share invitation.\"\n    },\n    \"is_member\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the calling user is a member of this conversation.\"\n    },\n    \"is_open\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DM is open.\"\n    },\n    \"is_frozen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is frozen.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the conversation was created.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the member who created this channel.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the last update to the conversation.\"\n    },\n    \"unlinked\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of times the channel has been unlinked.\"\n    },\n    \"topic\": {\n      \"type\": \"object\",\n      \"description\": \"The channel topic.\"\n    },\n    \"purpose\": {\n      \"type\": \"object\",\n      \"description\": \"The channel purpose.\"\n    },\n    \"previous_names\": {\n      \"type\": \"array\",\n      \"description\": \"A list of previous names the channel had.\"\n    },\n    \"num_members\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of members in the channel. Only included when specifically requested.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"IETF language code for the channel locale. Only included when specifically requested.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"For direct messages, the user ID of the other participant.\"\n    },\n    \"shared_team_ids\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Array of team IDs that share this channel (for shared channels).\"\n    },\n    \"parent_conversation\": {\n      \"type\": \"string\",\n      \"description\": \"Parent conversation ID for thread-only channels.\"\n    },\n    \"context_team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace team ID.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional channel properties.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-channel-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: Channel
---
