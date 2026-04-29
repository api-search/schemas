---
description: Represents a conversation inbox configuration where messages are organized and routed.
layout: schema
name: Inbox
properties_list:
- description: Unique identifier for the inbox
  name: id
  type: string
- description: Display name of the inbox
  name: name
  type: string
- description: Type of inbox (e.g., CONVERSATIONS_INBOX)
  name: type
  type: string
- description: ISO 8601 timestamp when the inbox was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the inbox was last updated
  name: updatedAt
  type: string
- description: Whether the inbox is archived
  name: archived
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-inbox-schema.json
slug: hubspot-conversations-inbox
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a conversation inbox configuration where messages are organized and routed.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the inbox\",\n      \"example\": \"12345678\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the inbox\",\n      \"example\": \"Support Inbox\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of inbox (e.g., CONVERSATIONS_INBOX)\",\n      \"example\": \"CONVERSATIONS_INBOX\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the inbox was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-10T09:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the inbox was last updated\",\n      \"format\": \"\
  date-time\",\n      \"example\": \"2024-01-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the inbox is archived\",\n      \"example\": false\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"createdAt\",\n    \"updatedAt\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Inbox\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-inbox-schema.json
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
title: Inbox
---
