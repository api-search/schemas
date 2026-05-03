---
description: A message sent in a Sendbird channel.
layout: schema
name: Sendbird Message
properties_list:
- description: Unique identifier of the message.
  name: message_id
  type: integer
- description: 'Type of message: MESG (text), FILE (file), ADMM (admin).'
  name: type
  type: string
- description: Text content of the message.
  name: message
  type: string
- description: URL of the channel containing this message.
  name: channel_url
  type: string
- description: Unix timestamp (milliseconds) when the message was sent.
  name: created_at
  type: integer
- description: Unix timestamp (milliseconds) when the message was last updated.
  name: updated_at
  type: integer
- description: Custom type for message categorization.
  name: custom_type
  type: string
- description: Custom data string attached to the message.
  name: data
  type: string
- description: 'Type of user mention: ''users'' for specific users, ''channel'' for all members.'
  name: mention_type
  type: string
- description: Users mentioned in the message.
  name: mentioned_users
  type: array
provider_name: Sendbird
provider_slug: sendbird
schema_file: json-schema/sendbird-message-schema.json
slug: sendbird-message
source_filename: sendbird-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sendbird/json-schema/sendbird-message-schema.json\",\n  \"title\": \"Sendbird Message\",\n  \"description\": \"A message sent in a Sendbird channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the message.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of message: MESG (text), FILE (file), ADMM (admin).\",\n      \"enum\": [\"MESG\", \"FILE\", \"ADMM\"]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the message.\"\n    },\n    \"channel_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the channel containing this message.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (milliseconds) when the message\
  \ was sent.\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (milliseconds) when the message was last updated.\"\n    },\n    \"custom_type\": {\n      \"type\": \"string\",\n      \"description\": \"Custom type for message categorization.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Custom data string attached to the message.\"\n    },\n    \"mention_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of user mention: 'users' for specific users, 'channel' for all members.\",\n      \"enum\": [\"users\", \"channel\"]\n    },\n    \"mentioned_users\": {\n      \"type\": \"array\",\n      \"description\": \"Users mentioned in the message.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"user_id\": {\"type\": \"string\"},\n          \"nickname\": {\"type\": \"string\"}\n        }\n      }\n    }\n  },\n  \"required\": [\"message_id\", \"\
  type\", \"channel_url\", \"created_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sendbird/refs/heads/main/json-schema/sendbird-message-schema.json
tags: []
title: Sendbird Message
---
