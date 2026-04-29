---
description: Paginated collection of conversation threads
layout: schema
name: ThreadCollection
properties_list:
- description: Array of thread records
  name: results
  type: array
- description: Pagination information for list responses.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-thread-collection-schema.json
slug: conversations-api-thread-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-thread-collection-schema.json\",\n  \"title\": \"ThreadCollection\",\n  \"description\": \"Paginated collection of conversation threads\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a conversation thread containing messages between participants.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the thread\",\n            \"example\": \"987654321\"\n          },\n          \"inboxId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the inbox containing this thread\",\n            \"example\": \"12345678\"\n          },\n          \"status\"\
  : {\n            \"type\": \"string\",\n            \"enum\": [\n              \"OPEN\",\n              \"CLOSED\"\n            ],\n            \"description\": \"Current status of the thread\",\n            \"example\": \"OPEN\"\n          },\n          \"spam\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the thread is marked as spam\",\n            \"example\": false\n          },\n          \"associatedContactId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the associated CRM contact\",\n            \"example\": \"101\"\n          },\n          \"assignedTo\": {\n            \"type\": \"string\",\n            \"description\": \"User ID the thread is assigned to\",\n            \"example\": \"user_456\"\n          },\n          \"originalChannelId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the original communication channel\",\n            \"example\": \"channel_789\"\n          },\n\
  \          \"originalChannelAccountId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the original channel account\",\n            \"example\": \"account_123\"\n          },\n          \"latestMessageTimestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp of the latest message\",\n            \"example\": \"2024-01-20T10:30:00Z\"\n          },\n          \"latestMessageSentTimestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp of the latest sent message\",\n            \"example\": \"2024-01-20T10:25:00Z\"\n          },\n          \"latestMessageReceivedTimestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp of the latest received message\",\n            \"example\": \"2024-01-20T10:30:00Z\"\n          },\n\
  \          \"closedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the thread was closed\",\n            \"example\": \"2024-01-21T15:00:00Z\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the thread was created\",\n            \"example\": \"2024-01-15T09:00:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the thread is archived\",\n            \"example\": false\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"inboxId\",\n          \"status\",\n          \"createdAt\"\n        ]\n      },\n      \"description\": \"Array of thread records\",\n      \"example\": [\n        {\n          \"id\": \"987654321\",\n          \"inboxId\": \"12345678\",\n          \"status\"\
  : \"OPEN\",\n          \"spam\": false,\n          \"associatedContactId\": \"101\",\n          \"assignedTo\": \"user_456\",\n          \"originalChannelId\": \"channel_789\",\n          \"originalChannelAccountId\": \"account_123\",\n          \"latestMessageTimestamp\": \"2024-01-20T10:30:00Z\",\n          \"latestMessageSentTimestamp\": \"2024-01-20T10:25:00Z\",\n          \"latestMessageReceivedTimestamp\": \"2024-01-20T10:30:00Z\",\n          \"closedAt\": \"2024-01-21T15:00:00Z\",\n          \"createdAt\": \"2024-01-15T09:00:00Z\",\n          \"archived\": false\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor information for retrieving the next page.\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n          \
  \    \"description\": \"Cursor token for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page\",\n              \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-thread-collection-schema.json
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
title: ThreadCollection
---
