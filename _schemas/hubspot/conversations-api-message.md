---
description: Represents a message within a conversation thread.
layout: schema
name: Message
properties_list:
- description: Unique identifier for the message
  name: id
  type: string
- description: Type of message
  name: type
  type: string
- description: Plain text content of the message
  name: text
  type: string
- description: Rich text (HTML) content of the message
  name: richText
  type: string
- description: Direction of the message (incoming or outgoing)
  name: direction
  type: string
- description: ID of the communication channel
  name: channelId
  type: string
- description: ID of the channel account
  name: channelAccountId
  type: string
- description: List of message senders
  name: senders
  type: array
- description: List of message recipients
  name: recipients
  type: array
- description: Delivery status information for a message
  name: status
  type: object
- description: ISO 8601 timestamp when the message was created
  name: createdAt
  type: string
- description: Whether the message was truncated
  name: truncationStatus
  type: string
- description: Message attachments
  name: attachments
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-message-schema.json
slug: conversations-api-message
source_filename: conversations-api-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Represents a message within a conversation thread.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the message\",\n      \"example\": \"msg_123456\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MESSAGE\",\n        \"COMMENT\",\n        \"WELCOME_MESSAGE\"\n      ],\n      \"description\": \"Type of message\",\n      \"example\": \"MESSAGE\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text content of the message\",\n      \"example\": \"Hello, I need help with my order.\"\n    },\n    \"richText\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Rich text (HTML) content of the message\",\n      \"example\": \"<p>Hello, I need help with my order.</p>\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INCOMING\",\n        \"OUTGOING\"\n      ],\n      \"description\": \"Direction of the message (incoming or outgoing)\",\n      \"example\": \"INCOMING\"\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the communication channel\",\n      \"example\": \"channel_789\"\n    },\n    \"channelAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the channel account\",\n      \"example\": \"account_123\"\n    },\n    \"senders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a participant in a conversation (visitor, agent, or bot).\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier\
  \ for the actor\",\n            \"example\": \"actor_101\"\n          },\n          \"actorId\": {\n            \"type\": \"string\",\n            \"description\": \"Actor ID reference\",\n            \"example\": \"actor_101\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the actor\",\n            \"example\": \"John Customer\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"Email address of the actor\",\n            \"example\": \"john@example.com\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of actor (e.g., VISITOR, AGENT, BOT)\",\n            \"example\": \"VISITOR\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"List of message senders\",\n      \"example\": [\n        {\n          \"id\"\
  : \"actor_101\",\n          \"actorId\": \"actor_101\",\n          \"name\": \"John Customer\",\n          \"email\": \"john@example.com\",\n          \"type\": \"VISITOR\"\n        }\n      ]\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a participant in a conversation (visitor, agent, or bot).\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the actor\",\n            \"example\": \"actor_101\"\n          },\n          \"actorId\": {\n            \"type\": \"string\",\n            \"description\": \"Actor ID reference\",\n            \"example\": \"actor_101\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the actor\",\n            \"example\": \"John Customer\"\n          },\n          \"email\": {\n            \"type\":\
  \ \"string\",\n            \"format\": \"email\",\n            \"description\": \"Email address of the actor\",\n            \"example\": \"john@example.com\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of actor (e.g., VISITOR, AGENT, BOT)\",\n            \"example\": \"VISITOR\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"List of message recipients\",\n      \"example\": [\n        {\n          \"id\": \"actor_101\",\n          \"actorId\": \"actor_101\",\n          \"name\": \"John Customer\",\n          \"email\": \"john@example.com\",\n          \"type\": \"VISITOR\"\n        }\n      ]\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"Delivery status information for a message\",\n      \"properties\": {\n        \"statusType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SENT\",\n      \
  \      \"DELIVERED\",\n            \"READ\",\n            \"FAILED\"\n          ],\n          \"description\": \"Current delivery status type\",\n          \"example\": \"DELIVERED\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message was created\",\n      \"example\": \"2024-01-20T10:30:00Z\"\n    },\n    \"truncationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the message was truncated\",\n      \"example\": \"NOT_TRUNCATED\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a file attachment on a message.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the attachment\",\n            \"example\": \"attach_001\"\n          },\n          \"type\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"MIME type of the attachment\",\n            \"example\": \"application/pdf\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL to access the attachment\",\n            \"example\": \"https://api.hubapi.com/files/v3/files/attach_001\"\n          },\n          \"filename\": {\n            \"type\": \"string\",\n            \"description\": \"Original filename\",\n            \"example\": \"invoice.pdf\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"File size in bytes\",\n            \"example\": 102400\n          }\n        }\n      },\n      \"description\": \"Message attachments\",\n      \"example\": [\n        {\n          \"id\": \"attach_001\",\n          \"type\": \"application/pdf\",\n          \"url\": \"https://api.hubapi.com/files/v3/files/attach_001\",\n    \
  \      \"filename\": \"invoice.pdf\",\n          \"size\": 102400\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-message-schema.json
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
title: Message
---
