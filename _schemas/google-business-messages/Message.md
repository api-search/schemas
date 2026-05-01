---
description: A message sent or received through the Google Business Messages API.
layout: schema
name: Google Business Message
properties_list:
- description: Resource name of the message.
  name: name
  type: string
- description: Unique identifier of the message.
  name: messageId
  type: string
- description: The representative sending the message.
  name: representative
  type: object
- description: Text content of the message.
  name: text
  type: string
- description: Rich card content.
  name: richCard
  type: object
- description: Suggested replies or actions.
  name: suggestions
  type: array
- description: Fallback text for unsupported clients.
  name: fallback
  type: string
- description: Whether the message contains rich text.
  name: containsRichText
  type: boolean
- description: Timestamp of message creation.
  name: createTime
  type: string
provider_name: Google Business Messages
provider_slug: google-business-messages
schema_file: json-schema/Message.json
slug: Message
source_filename: Message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"Message.json\",\n  \"title\": \"Google Business Message\",\n  \"description\": \"A message sent or received through the Google Business Messages API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the message.\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the message.\"\n    },\n    \"representative\": {\n      \"type\": \"object\",\n      \"description\": \"The representative sending the message.\",\n      \"properties\": {\n        \"representativeType\": {\n          \"type\": \"string\",\n          \"enum\": [\"BOT\", \"HUMAN\"]\n        },\n        \"displayName\": {\n          \"type\": \"string\"\n        },\n        \"avatarImage\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"text\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Text content of the message.\"\n    },\n    \"richCard\": {\n      \"type\": \"object\",\n      \"description\": \"Rich card content.\"\n    },\n    \"suggestions\": {\n      \"type\": \"array\",\n      \"description\": \"Suggested replies or actions.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"fallback\": {\n      \"type\": \"string\",\n      \"description\": \"Fallback text for unsupported clients.\"\n    },\n    \"containsRichText\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the message contains rich text.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of message creation.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-business-messages/refs/heads/main/json-schema/Message.json
tags:
- Business Communications
- Conversations
- Customer Support
- Google
- Messaging
title: Google Business Message
---
