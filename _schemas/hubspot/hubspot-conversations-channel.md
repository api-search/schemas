---
description: Represents a communication channel for conversations.
layout: schema
name: Channel
properties_list:
- description: Unique identifier for the channel
  name: id
  type: string
- description: Display name of the channel
  name: name
  type: string
- description: Type of channel (e.g., EMAIL, CHAT, FACEBOOK)
  name: type
  type: string
- description: Associated account ID
  name: accountId
  type: string
- description: ISO 8601 timestamp when the channel was created
  name: createdAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-channel-schema.json
slug: hubspot-conversations-channel
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a communication channel for conversations.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the channel\",\n      \"example\": \"channel_789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the channel\",\n      \"example\": \"Website Chat\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of channel (e.g., EMAIL, CHAT, FACEBOOK)\",\n      \"example\": \"CHAT\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated account ID\",\n      \"example\": \"account_123\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the channel was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-01T00:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"\
  name\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Channel\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-channel-schema.json
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
title: Channel
---
