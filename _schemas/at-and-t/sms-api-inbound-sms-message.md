---
description: InboundSmsMessage schema from AT&T API
layout: schema
name: InboundSmsMessage
properties_list:
- description: Unique identifier for the inbound message
  name: messageId
  type: string
- description: SMS message text content
  name: message
  type: string
- description: Phone number of the message sender in tel:+E.164 format
  name: senderAddress
  type: string
- description: Short code that received the message
  name: destinationAddress
  type: string
- description: Date and time when the message was received
  name: dateTime
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-inbound-sms-message-schema.json
slug: sms-api-inbound-sms-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-inbound-sms-message-schema.json\",\n  \"title\": \"InboundSmsMessage\",\n  \"description\": \"InboundSmsMessage schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the inbound message\",\n      \"example\": \"msg-500456\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"SMS message text content\",\n      \"example\": \"STOP\"\n    },\n    \"senderAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the message sender in tel:+E.164 format\",\n      \"example\": \"tel:+12125551234\"\n    },\n    \"destinationAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Short code that received the message\",\n      \"\
  example\": \"12345\"\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the message was received\",\n      \"example\": \"2026-04-19T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-inbound-sms-message-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: InboundSmsMessage
---
