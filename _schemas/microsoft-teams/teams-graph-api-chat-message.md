---
description: Represents a message in a channel or chat.
layout: schema
name: ChatMessage
properties_list:
- description: Unique identifier for the message.
  name: id
  type: string
- description: When the message was created.
  name: createdDateTime
  type: string
- description: When the message was last modified.
  name: lastModifiedDateTime
  type: string
- description: The type of message.
  name: messageType
  type: string
- description: Message importance.
  name: importance
  type: string
- description: Subject of the message.
  name: subject
  type: string
- description: Message body content.
  name: body
  type: object
- description: Sender information.
  name: from
  type: object
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-chat-message-schema.json
slug: teams-graph-api-chat-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-chat-message-schema.json\",\n  \"title\": \"ChatMessage\",\n  \"description\": \"Represents a message in a channel or chat.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the message.\" },\n    \"createdDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"When the message was created.\" },\n    \"lastModifiedDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"When the message was last modified.\" },\n    \"messageType\": { \"type\": \"string\", \"enum\": [\"message\", \"chatEvent\", \"typing\", \"unknownFutureValue\", \"systemEventMessage\"], \"description\": \"The type of message.\" },\n    \"importance\": { \"type\": \"string\", \"enum\": [\"normal\"\
  , \"high\", \"urgent\"], \"description\": \"Message importance.\" },\n    \"subject\": { \"type\": \"string\", \"description\": \"Subject of the message.\" },\n    \"body\": {\n      \"type\": \"object\",\n      \"description\": \"Message body content.\",\n      \"properties\": {\n        \"contentType\": { \"type\": \"string\", \"enum\": [\"text\", \"html\"] },\n        \"content\": { \"type\": \"string\" }\n      }\n    },\n    \"from\": {\n      \"type\": \"object\",\n      \"description\": \"Sender information.\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": { \"type\": \"string\" },\n            \"displayName\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-chat-message-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: ChatMessage
---
