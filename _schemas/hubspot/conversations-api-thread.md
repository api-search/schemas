---
description: Represents a conversation thread containing messages between participants.
layout: schema
name: Thread
properties_list:
- description: Unique identifier for the thread
  name: id
  type: string
- description: ID of the inbox containing this thread
  name: inboxId
  type: string
- description: Current status of the thread
  name: status
  type: string
- description: Whether the thread is marked as spam
  name: spam
  type: boolean
- description: ID of the associated CRM contact
  name: associatedContactId
  type: string
- description: User ID the thread is assigned to
  name: assignedTo
  type: string
- description: ID of the original communication channel
  name: originalChannelId
  type: string
- description: ID of the original channel account
  name: originalChannelAccountId
  type: string
- description: ISO 8601 timestamp of the latest message
  name: latestMessageTimestamp
  type: string
- description: ISO 8601 timestamp of the latest sent message
  name: latestMessageSentTimestamp
  type: string
- description: ISO 8601 timestamp of the latest received message
  name: latestMessageReceivedTimestamp
  type: string
- description: ISO 8601 timestamp when the thread was closed
  name: closedAt
  type: string
- description: ISO 8601 timestamp when the thread was created
  name: createdAt
  type: string
- description: Whether the thread is archived
  name: archived
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-thread-schema.json
slug: conversations-api-thread
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-thread-schema.json\",\n  \"title\": \"Thread\",\n  \"description\": \"Represents a conversation thread containing messages between participants.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the thread\",\n      \"example\": \"987654321\"\n    },\n    \"inboxId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the inbox containing this thread\",\n      \"example\": \"12345678\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\"\n      ],\n      \"description\": \"Current status of the thread\",\n      \"example\": \"OPEN\"\n    },\n    \"spam\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the thread\
  \ is marked as spam\",\n      \"example\": false\n    },\n    \"associatedContactId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the associated CRM contact\",\n      \"example\": \"101\"\n    },\n    \"assignedTo\": {\n      \"type\": \"string\",\n      \"description\": \"User ID the thread is assigned to\",\n      \"example\": \"user_456\"\n    },\n    \"originalChannelId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the original communication channel\",\n      \"example\": \"channel_789\"\n    },\n    \"originalChannelAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the original channel account\",\n      \"example\": \"account_123\"\n    },\n    \"latestMessageTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the latest message\",\n      \"example\": \"2024-01-20T10:30:00Z\"\n    },\n    \"latestMessageSentTimestamp\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the latest sent message\",\n      \"example\": \"2024-01-20T10:25:00Z\"\n    },\n    \"latestMessageReceivedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the latest received message\",\n      \"example\": \"2024-01-20T10:30:00Z\"\n    },\n    \"closedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the thread was closed\",\n      \"example\": \"2024-01-21T15:00:00Z\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the thread was created\",\n      \"example\": \"2024-01-15T09:00:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the thread is archived\",\n      \"example\": false\n    }\n  },\n  \"required\": [\n \
  \   \"id\",\n    \"inboxId\",\n    \"status\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-thread-schema.json
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
title: Thread
---
