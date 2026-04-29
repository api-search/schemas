---
description: Request payload for sending a message to a thread.
layout: schema
name: SendMessageRequest
properties_list:
- description: Type of message to send
  name: type
  type: string
- description: Plain text content of the message
  name: text
  type: string
- description: Rich text (HTML) content
  name: richText
  type: string
- description: Actor ID of the sender
  name: senderActorId
  type: string
- description: Channel to send on
  name: channelId
  type: string
- description: Channel account to use
  name: channelAccountId
  type: string
- description: Message recipients
  name: recipients
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-send-message-request-schema.json
slug: conversations-api-send-message-request
source_filename: conversations-api-send-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-send-message-request-schema.json\",\n  \"title\": \"SendMessageRequest\",\n  \"description\": \"Request payload for sending a message to a thread.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MESSAGE\",\n        \"COMMENT\"\n      ],\n      \"description\": \"Type of message to send\",\n      \"example\": \"MESSAGE\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text content of the message\",\n      \"example\": \"Thank you for reaching out. How can I help you today?\"\n    },\n    \"richText\": {\n      \"type\": \"string\",\n      \"description\": \"Rich text (HTML) content\",\n      \"example\": \"<p>Thank you for reaching out. How can I help you today?</p>\"\n    },\n  \
  \  \"senderActorId\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID of the sender\",\n      \"example\": \"actor_agent_123\"\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"Channel to send on\",\n      \"example\": \"channel_789\"\n    },\n    \"channelAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Channel account to use\",\n      \"example\": \"account_123\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Recipient information for a message.\",\n        \"properties\": {\n          \"actorId\": {\n            \"type\": \"string\",\n            \"description\": \"Actor ID of the recipient\",\n            \"example\": \"actor_101\"\n          }\n        }\n      },\n      \"description\": \"Message recipients\",\n      \"example\": [\n        {\n          \"actorId\": \"actor_101\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"type\",\n    \"text\",\n    \"senderActorId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-send-message-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: SendMessageRequest
---
