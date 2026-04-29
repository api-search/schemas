---
description: A Slack message object representing a single message in a conversation. Messages can contain text, blocks, attachments, files, and reactions.
layout: schema
name: Message
properties_list:
- description: Always "message" for messages.
  name: type
  type: string
- description: Optional subtype indicating a specialized message type such as bot_message, channel_join, channel_leave, etc.
  name: subtype
  type: string
- description: The channel ID where the message was posted.
  name: channel
  type: string
- description: The user ID of the message author.
  name: user
  type: string
- description: The text content of the message.
  name: text
  type: string
- description: Unique timestamp identifier for the message, also serves as the message ID. Format is Unix epoch with microseconds (e.g., "1503435956.000247").
  name: ts
  type: string
- description: The timestamp of the parent message in a thread. Present only for threaded replies.
  name: thread_ts
  type: string
- description: Number of replies in the thread.
  name: reply_count
  type: integer
- description: Number of unique users who have replied in the thread.
  name: reply_users_count
  type: integer
- description: Timestamp of the most recent reply in the thread.
  name: latest_reply
  type: string
- description: Array of user IDs who have replied in the thread.
  name: reply_users
  type: array
- description: An array of Block Kit layout blocks used for rich message formatting.
  name: blocks
  type: array
- description: An array of message attachments.
  name: attachments
  type: array
- description: An array of file objects attached to the message.
  name: files
  type: array
- description: An array of emoji reactions on this message.
  name: reactions
  type: array
- description: Edit information if the message was edited.
  name: edited
  type: object
- description: Bot ID if the message was posted by a bot.
  name: bot_id
  type: string
- description: Bot profile information if posted by a bot.
  name: bot_profile
  type: object
- description: Custom metadata attached to the message by an application.
  name: metadata
  type: object
- description: Permalink URL for the message.
  name: permalink
  type: string
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-message-schema.json
slug: slack-web-message
source_filename: slack-web-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Message\",\n  \"type\": \"object\",\n  \"description\": \"A Slack message object representing a single message in a conversation. Messages can contain text, blocks, attachments, files, and reactions.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Always \\\"message\\\" for messages.\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Optional subtype indicating a specialized message type such as bot_message, channel_join, channel_leave, etc.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The channel ID where the message was posted.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the message author.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the message.\"\n    },\n  \
  \  \"ts\": {\n      \"type\": \"string\",\n      \"description\": \"Unique timestamp identifier for the message, also serves as the message ID. Format is Unix epoch with microseconds (e.g., \\\"1503435956.000247\\\").\"\n    },\n    \"thread_ts\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the parent message in a thread. Present only for threaded replies.\"\n    },\n    \"reply_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of replies in the thread.\"\n    },\n    \"reply_users_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique users who have replied in the thread.\"\n    },\n    \"latest_reply\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the most recent reply in the thread.\"\n    },\n    \"reply_users\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user IDs who have replied in the thread.\"\n    },\n    \"blocks\": {\n      \"type\": \"array\",\n\
  \      \"description\": \"An array of Block Kit layout blocks used for rich message formatting.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"An array of message attachments.\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"An array of file objects attached to the message.\"\n    },\n    \"reactions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of emoji reactions on this message.\"\n    },\n    \"edited\": {\n      \"type\": \"object\",\n      \"description\": \"Edit information if the message was edited.\"\n    },\n    \"bot_id\": {\n      \"type\": \"string\",\n      \"description\": \"Bot ID if the message was posted by a bot.\"\n    },\n    \"bot_profile\": {\n      \"type\": \"object\",\n      \"description\": \"Bot profile information if posted by a bot.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata attached to the message by an\
  \ application.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"description\": \"Permalink URL for the message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-message-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: Message
---
