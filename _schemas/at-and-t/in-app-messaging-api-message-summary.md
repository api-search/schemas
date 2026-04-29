---
description: MessageSummary schema from AT&T API
layout: schema
name: MessageSummary
properties_list:
- description: Unique message identifier
  name: messageId
  type: string
- description: Sender address (phone number or email)
  name: from
  type: string
- description: List of recipient addresses
  name: recipients
  type: array
- description: Whether the message has been read
  name: isUnread
  type: boolean
- description: True if message was received, false if sent
  name: isIncoming
  type: boolean
- description: Message type
  name: type
  type: string
- description: Numeric type code
  name: typeCode
  type: string
- description: Date and time the message was sent or received
  name: timeStamp
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/in-app-messaging-api-message-summary-schema.json
slug: in-app-messaging-api-message-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-summary-schema.json\",\n  \"title\": \"MessageSummary\",\n  \"description\": \"MessageSummary schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique message identifier\",\n      \"example\": \"msg-500123\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Sender address (phone number or email)\",\n      \"example\": \"tel:+12125551234\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"List of recipient addresses\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"tel:+12125559999\"\n      ]\n    },\n    \"isUnread\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether the message has been read\",\n      \"example\": false\n    },\n    \"isIncoming\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if message was received, false if sent\",\n      \"example\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Message type\",\n      \"enum\": [\n        \"TEXT\",\n        \"MMS\"\n      ],\n      \"example\": \"TEXT\"\n    },\n    \"typeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Numeric type code\",\n      \"example\": \"1\"\n    },\n    \"timeStamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the message was sent or received\",\n      \"example\": \"2026-04-19T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/in-app-messaging-api-message-summary-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: MessageSummary
---
