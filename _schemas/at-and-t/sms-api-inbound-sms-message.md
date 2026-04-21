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
