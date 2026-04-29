---
description: Paginated collection of inboxes
layout: schema
name: InboxCollection
properties_list:
- description: Array of inbox records
  name: results
  type: array
- description: Total number of inboxes available
  name: total
  type: integer
- description: Pagination information for list responses.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-inbox-collection-schema.json
slug: hubspot-conversations-inbox-collection
source_filename: hubspot-conversations-inbox-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of inboxes\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of inbox records\",\n      \"example\": [\n        {\n          \"id\": \"12345678\",\n          \"name\": \"Support Inbox\",\n          \"type\": \"CONVERSATIONS_INBOX\",\n          \"createdAt\": \"2024-01-10T09:00:00Z\",\n          \"updatedAt\": \"2024-01-15T14:30:00Z\",\n          \"archived\": false\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a conversation inbox configuration where messages are organized and routed.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the inbox\",\n            \"example\": \"12345678\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name\
  \ of the inbox\",\n            \"example\": \"Support Inbox\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of inbox (e.g., CONVERSATIONS_INBOX)\",\n            \"example\": \"CONVERSATIONS_INBOX\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the inbox was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-10T09:00:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the inbox was last updated\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the inbox is archived\",\n            \"example\": false\n          }\n        },\n        \"required\": [\n          \"\
  id\",\n          \"name\",\n          \"createdAt\",\n          \"updatedAt\"\n        ]\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of inboxes available\",\n      \"example\": 2\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor information for retrieving the next page.\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page\",\n              \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n            }\n       \
  \   }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InboxCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-inbox-collection-schema.json
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
title: InboxCollection
---
