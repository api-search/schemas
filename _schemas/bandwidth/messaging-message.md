---
description: Message schema from Bandwidth messaging API
layout: schema
name: Message
properties_list:
- description: The unique identifier for the message
  name: id
  type: string
- description: The Bandwidth phone number that owns the message
  name: owner
  type: string
- description: The application ID associated with this message
  name: applicationId
  type: string
- description: The time the message was created
  name: time
  type: string
- description: The number of segments the message was split into
  name: segmentCount
  type: integer
- description: The direction of the message
  name: direction
  type: string
- description: The destination phone numbers
  name: to
  type: array
- description: The source phone number
  name: from
  type: string
- description: Media URLs attached to the message
  name: media
  type: array
- description: The text content of the message
  name: text
  type: string
- description: Custom tag attached to the message
  name: tag
  type: string
- description: The priority of the message
  name: priority
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-message-schema.json
slug: messaging-message
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Message
---
