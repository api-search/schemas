---
description: Paginated collection of channels
layout: schema
name: ChannelCollection
properties_list:
- description: Array of channel records
  name: results
  type: array
- description: Pagination information for list responses.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-channel-collection-schema.json
slug: conversations-api-channel-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-channel-collection-schema.json\",\n  \"title\": \"ChannelCollection\",\n  \"description\": \"Paginated collection of channels\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a communication channel for conversations.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the channel\",\n            \"example\": \"channel_789\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the channel\",\n            \"example\": \"Website Chat\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"Type of channel (e.g., EMAIL, CHAT, FACEBOOK)\",\n            \"example\": \"CHAT\"\n          },\n          \"accountId\": {\n            \"type\": \"string\",\n            \"description\": \"Associated account ID\",\n            \"example\": \"account_123\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the channel was created\",\n            \"example\": \"2024-01-01T00:00:00Z\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\",\n          \"type\"\n        ]\n      },\n      \"description\": \"Array of channel records\",\n      \"example\": [\n        {\n          \"id\": \"channel_789\",\n          \"name\": \"Website Chat\",\n          \"type\": \"CHAT\",\n          \"accountId\": \"account_123\",\n          \"createdAt\": \"2024-01-01T00:00:00Z\"\n        }\n      ]\n    },\n    \"paging\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor information for retrieving the next page.\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page\",\n              \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-channel-collection-schema.json
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
title: ChannelCollection
---
