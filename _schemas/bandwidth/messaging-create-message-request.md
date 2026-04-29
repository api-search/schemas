---
description: CreateMessageRequest schema from Bandwidth messaging API
layout: schema
name: CreateMessageRequest
properties_list:
- description: The Bandwidth phone number to send the message from, in E.164 format
  name: from
  type: string
- description: Array of destination phone numbers in E.164 format. Up to 50 numbers for group messaging.
  name: to
  type: array
- description: The text content of the message. Required for SMS. For MMS, text is optional if media is provided.
  name: text
  type: string
- description: Array of media URLs to include as MMS attachments. Each URL must be publicly accessible or a Bandwidth media URL.
  name: media
  type: array
- description: The ID of the Bandwidth application associated with this message. This determines which webhook URLs receive delivery callbacks.
  name: applicationId
  type: string
- description: A custom string to attach to the message for tracking purposes
  name: tag
  type: string
- description: The priority of the message. High priority messages are delivered faster but may incur additional charges.
  name: priority
  type: string
- description: The expiration time for the message. Messages not delivered by this time will be discarded.
  name: expiration
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-create-message-request-schema.json
slug: messaging-create-message-request
source_filename: messaging-create-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-create-message-request-schema.json\",\n  \"title\": \"CreateMessageRequest\",\n  \"description\": \"CreateMessageRequest schema from Bandwidth messaging API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth phone number to send the message from, in E.164 format\",\n      \"example\": \"+19195551234\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 50,\n      \"description\": \"Array of destination phone numbers in E.164 format. Up to 50 numbers for group messaging.\",\n      \"example\": [\n        \"+19195554321\"\n      ]\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n  \
  \    \"description\": \"The text content of the message. Required for SMS. For MMS, text is optional if media is provided.\"\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"Array of media URLs to include as MMS attachments. Each URL must be publicly accessible or a Bandwidth media URL.\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Bandwidth application associated with this message. This determines which webhook URLs receive delivery callbacks.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"A custom string to attach to the message for tracking purposes\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"default\",\n        \"high\"\n      ],\n      \"default\": \"default\",\n      \"description\": \"The priority of the message. High priority\
  \ messages are delivered faster but may incur additional charges.\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The expiration time for the message. Messages not delivered by this time will be discarded.\"\n    }\n  },\n  \"required\": [\n    \"from\",\n    \"to\",\n    \"text\",\n    \"applicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-create-message-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: CreateMessageRequest
---
