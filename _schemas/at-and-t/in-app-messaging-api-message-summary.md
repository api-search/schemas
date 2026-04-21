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
